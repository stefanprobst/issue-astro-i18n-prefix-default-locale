when `prefixDefaultLocale` is set to `true`, it is not possible to reach an unprefixed route, e.g. one injected by an integration.

in the minimal issue reproduction, i am trying to reach `/keystatic`, defined in `src/pages/keystatic.astro`.

my actual issue is: i am using the [keystatic cms astro integration](https://keystatic.com/docs/installation-astro), which injects the unprefixed `/keystatic` route [here](https://github.com/Thinkmill/keystatic/blob/main/packages/astro/src/index.ts#L44-L50).
