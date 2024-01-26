# ephiframe

> ephimeral iframe page builder

Build your own pages via URL, use one of these domains:

- https://ephiframe.vercel.app
- https://b-ephiframe.vercel.app
- https://alt-ephiframe.vercel.app
- https://more-ephiframe.vercel.app
- https://extra-ephiframe.vercel.app
- https://static-ephiframe.vercel.app
- https://dynamic-ephiframe.vercel.app
- https://accepted-ephiframe.vercel.app
- https://excluded-ephiframe.vercel.app

Then add titles and descriptions via pathname, like:

- [/base-test-also-used-as-title](https://ephiframe.vercel.app/base-test-also-used-as-title)
- [/domain-test/The-last-part-is-used-as-title](https://more-ephiframe.vercel.app/domain-test/The-last-part-is-used-as-title)

Then add any number of `iframe` search aparameters to create multiple frames on the page, even across domains:

- [?iframe=./Custom-title](https://more-ephiframe.vercel.app/Outer?iframe=./Custom-title)
- [?iframe=./Custom-title&iframe=./Other-iframe](https://extra-ephiframe.vercel.app/Outer?iframe=./Custom-title&iframe=./Other-iframe)
- [?iframe=https://extra-ephiframe.vercel.app/Cross-domain-iframe](https://alt-ephiframe.vercel.app/Outer?iframe=https://extra-ephiframe.vercel.app/Cross-domain-iframe)
- [?iframe=https://extra-ephiframe.vercel.app/Cross-domain-iframe%3Fiframe%3D./nested](https://ephiframe.vercel.app/Outer?iframe=https://extra-ephiframe.vercel.app/Cross-domain-iframe%3Fiframe%3D./nested)
- [?iframe=https://extra-ephiframe.vercel.app/Brix%3Fiframe%3Dhttps%3A%2F%2Fephiframe.vercel.app%2FPixie](https://ephiframe.vercel.app/Pixie?iframe=https://extra-ephiframe.vercel.app/Brix%3Fiframe%3Dhttps%3A%2F%2Fephiframe.vercel.app%2FPixie)

And/or add any number of `srcdoc` search parameters with HTML:

- [?srcdoc=&lt;h1&gt;hello-srcdoc&srcdoc=&lt;ol&gt;&lt;li&gt;second](https://ephiframe.vercel.app/?srcdoc=%3Ch1%3Ehello-srcdoc&srcdoc=%3Col%3E%3Cli%3Esecond)

You can add any `sandbox` search parameter that will be added in order to the generated iframes (regular `iframe` parameters are always processed before `srcdoc`). An empty `sandbox=` parameter applies the full sandbox, equivalent to `sandbox=""` in HTML.

- [?sandbox=&iframe=./Full-sandbox](https://ephiframe.vercel.app/Outer?sandbox=&iframe=./Full-sandbox)
- [?sandbox=allow-scripts&iframe=./Allow-scripts](https://extra-ephiframe.vercel.app/Outer?sandbox=allow-scripts&iframe=./Allow-scripts)
- [?sandbox=&iframe=./Full-sandbox&iframe=./No-sandbox](https://more-ephiframe.vercel.app/Outer?sandbox=&iframe=./Full-sandbox&iframe=./No-sandbox)
- [?sandbox=&srcdoc=&lt;h1&gt;Sandboxed%20srcdoc&srcdoc=&lt;h1&gt;Free%20srcdoc](https://ephiframe.vercel.app/?sandbox=&srcdoc=%3Ch1%3ESandboxed%20srcdoc&srcdoc=%3Ch1%3EFree%20srcdoc)
