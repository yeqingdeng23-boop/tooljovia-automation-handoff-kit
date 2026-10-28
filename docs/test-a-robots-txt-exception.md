# Test a robots.txt exception before you publish it

You have a robots.txt rule that blocks a directory, but you want a crawler to reach one help page inside it. How can you tell which rule wins for that path? This short, fictional example walks through the decision before you change a live file.

I work on ToolJovia, which makes the free [Robots.txt Rule Tester](https://tooljovia.com/tools/robots-txt-tester/). It needs no account and processes the pasted rules in your browser tab. Use public or non-sensitive rules and paths for this exercise.

## The example

Imagine a site with these rules:

```text
User-agent: *
Disallow: /private/
Allow: /private/help$
```

The `*` group applies to the crawler token in this example. The first path rule covers the `/private/` directory. The second creates an exception for the exact path `/private/help`; its final `$` marks the end of the path. For this illustration, the expected decision for `ExampleBot` on `/private/help` is **Allow**. The more specific matching Allow rule wins over the broader Disallow rule.

For comparison, the expected decision for `/private/notes` is **Disallow**: the directory rule matches, while the exact help-page exception does not. These are example expectations, not a claim that either path exists or that a crawler has visited it.

## Try it step by step

1. Open the [tester](https://tooljovia.com/tools/robots-txt-tester/) and paste the three example lines into the robots.txt input. Paste the contents of the file, not the URL of the file.
2. Enter `ExampleBot` in the crawler or user-agent field.
3. Enter `/private/help` as the path and run the test.
4. Read the decision and the matching-rule trace. The expected result is Allow; look for the `Allow: /private/help$` rule and compare it with the matching `Disallow: /private/` rule.
5. Change only the path to `/private/notes` and run the test again. The expected result is Disallow. Check the trace to see which rule matched and whether the exception applied.

If your result differs, check the path spelling, the final `$`, the crawler token, and whether the rules were pasted into the intended group. For your own file, keep the surrounding user-agent groups intact: the group selected for a crawler can change the outcome. Review the full trace rather than assuming that the first matching line wins.

## What the result does and does not tell you

This tool evaluates the supplied text and path. It does not fetch your live robots.txt file, simulate HTTP fetch errors, or verify how a particular search engine will crawl or index a page. It reports unsupported extensions instead of applying them, and has limits including 2,000 input lines and 500 selected rules. Check the tool's own guidance for details before testing a large file.

An Allow result does not guarantee a crawl or a Google listing. A Disallow result is not a password or access control: crawlers may ignore it, and a blocked URL can still appear in search results. For private material, use appropriate access controls. If your goal is to keep a page out of Google Search, read Google's guidance on [robots.txt limitations](https://developers.google.com/search/docs/crawling-indexing/robots/intro) and [`noindex`](https://developers.google.com/search/docs/crawling-indexing/block-indexing); Google must be able to access a page to see its `noindex` instruction.

Before publishing a real change, compare the tested text with the file actually served by your site and check your search engine's documentation for its current behavior.

