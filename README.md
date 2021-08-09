# [Multisearch](https://szupie.github.io/multisearch/)
A web tool for displaying search results from multiple sources at the same time

To add a search engine / dictionary / lookup tool, enter its results page URL, replacing the query with `%s`. For example, `https://en.m.wiktionary.org/wiki/Special:Search?search=%s`

You can save/share sets of searches via the URL. Some example presets: 
- [look up a French word in Wiktionary and Reverso Context](https://szupie.github.io/multisearch/?engine=https%3A%2F%2Fen.m.wiktionary.org%2Fwiki%2F%25s%23French&engine=https%3A%2F%2Fcontext.reverso.net%2Ftranslation%2Ffrench-english%2F%25s)
- [look up the pronunciation in Cambridge Dictionary and the etymology on Etymonline.com](https://szupie.github.io/multisearch/?engine=https%3A%2F%2Fdictionary.cambridge.org%2Fpronunciation%2Fenglish%2F%25s%23entryContent&engine=https%3A%2F%2Fwww.etymonline.com%2Fsearch%3Fq%3D%25s)

## How it works
This uses iframes to load results from specified URLs. For security reasons, some sites do not allow embedding[1]. This means that **this tool will not work with Google, DuckDuckGo, MDN Web Docs, Forvo, or YouGlish**, just to name a few useful examples.

For security reasons, browsers do not allow http pages to be loaded on https pages[2]. If you want to use this with an http site, you can do so by running this locally – just download `index.html` and open it in your browser.

##### Footnotes
1. See [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options) on MDN
2. See [Mixed content](https://developer.mozilla.org/en-US/docs/Web/Security/Mixed_content) on MDN
