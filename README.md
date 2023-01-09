# ephiframe

> ephimeral iframe page builder

**Sponsored by [PixieBrix](https://www.pixiebrix.com)** :tada:

Build your own pages via URL, use one of these domains:

- https://ephiframe.vercel.app
- https://b-ephiframe.vercel.app
- https://alt-ephiframe.vercel.app
- https://more-ephiframe.vercel.app
- https://extra-ephiframe.vercel.app
- https://additional-ephiframe.vercel.app
- https://secondary-ephiframe.vercel.app
- https://supplementary-ephiframe.vercel.app

Then add titles and descriptions via pathname, like:

- [/base-test-also-used-as-title](https://ephiframe.vercel.app/base-test-also-used-as-title)
- [/domain-test/The-last-part-is-used-as-title](https://more-ephiframe.vercel.app/domain-test/The-last-part-is-used-as-title)

Then add any number of `iframe` search aparameters to create multiple frames on the page, even across domains:

- [?iframe=./Custom-title](https://more-ephiframe.vercel.app/Outer?iframe=./Custom-title)
- [?iframe=./Custom-title&iframe=./Other-iframe](https://extra-ephiframe.vercel.app/Outer?iframe=./Custom-title&iframe=./Other-iframe)
- [?iframe=https://extra-ephiframe.vercel.app/Cross-domain-iframe](https://alt-ephiframe.vercel.app/Outer?iframe=https://extra-ephiframe.vercel.app/Cross-domain-iframe)
- [?iframe=https://extra-ephiframe.vercel.app/Cross-domain-iframe%3Fiframe%3D./nested](https://ephiframe.vercel.app/Outer?iframe=https://extra-ephiframe.vercel.app/Cross-domain-iframe%3Fiframe%3D./nested)
