## Install

* pnpm add @vueuse/core
  * => some warms
```
pnpm add @vueuse/core
 WARN  2 deprecated subdependencies found: @npmcli/move-file@2.0.1, stable@0.1.8
Already up to date
Progress: resolved 981, reused 896, downloaded 0, added 0, done

dependencies:
+ @vueuse/core 10.6.1

 WARN  Issues with peer dependencies found
.
└─┬ astro-compress 2.2.3
  └─┬ typescript-esbuild 0.3.1
    └─┬ typedoc 0.25.2
      └── ✕ unmet peer typescript@"4.6.x || 4.7.x || 4.8.x || 4.9.x || 5.0.x || 5.1.x || 5.2.x": found 5.3.2

Done in 8.6s
``` 

* edit `src/layouts/BaseLayout.astro`
  * L. 108 : remove " s"
  * L. 97 : "src: contact.data.form.thumbnail," to "src: contact.data.form?.thumbnail,"
  * l. 81 : "src: contact.data.form.thumbnail," to "src: contact.data.form?.thumbnail,"
  * l. 25 : remove "<!doctype html>"

* edit `src/layouts/Footer.astro`
  * L. 119 : remove " opacity-60"


## Run

* pnpm run cms-proxy-server
* pnpm run dev:demo