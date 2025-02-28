---
layout: ~/layouts/MainLayout.astro
setup: |
  import Badge from '~/components/Badge.astro';
title: إعداد البيئة البرمجية
description: أعِد محرر الشفرة لبناء المشاريع مع Astro.
---

خصص محرر الكود لتحسين تجربة التطوير مع أسترو وفتح ميزات جديدة

## محرر VS Code

[محرر VS Code](https://code.visualstudio.com/) هو محرر شائع لمطوري الويب، من تطوير مايكروسوفت. نفس الكود الذي بُني عليه VS Code مستخدم لتشغيل المحررات الشائعة في المتصفح مثل [GitHub Codespaces](https://github.com/features/codespaces) و [Gitpod](https://gitpod.io/).

يعمل أسترو مع أي محرر ولكنّا نوصي باستخدام VS Code لمشاريع Astro. نُقدم الإضافة الرسمية [Astro VS Code](https://marketplace.visualstudio.com/items?itemName=astro-build.astro-vscode) التي تفتح العديد من الميزات الرئيسية، وتحسينات تجربة التطوير على أسترو.

- تلوين الكود (syntax highlighting) لملفات `.astro`.
- دعم الأنواع للغة TypeScript على ملفات `.astro`.
- [اقتراحات VS Code](https://code.visualstudio.com/docs/editor/intellisense) لإكمال الشفرة، والتلميحات وغيرها.

لنبدأ! ثبّت [الإضافة Astro VS Code](https://marketplace.visualstudio.com/items?itemName=astro-build.astro-vscode) الآن.

📚 راجع [اعداد دعم TypeScript](/ar/guides/typescript/) في مشاريع Astro.

## محررات برمجية أخرى

يقدم مجتمعنا المذهل عدة إضافات للمحررات الشهيرة الأخرى، بما في ذلك:

- [إضافة VS Code على Open VSX](https://open-vsx.org/extension/astro-build/astro-vscode) <span style="margin: 0.25em;"><Badge variant="accent">دعم رسمي</Badge></span> - إضافة VS Code الرسمية التي تحدثنا عنها أعلاه، متوفرة أيضا على مستودع Open VSX للمحررات المبنية عليه مثل [VSCodium](https://vscodium.com/)
- [إضافة Nova](https://extensions.panic.com/extensions/sciencefidelity/sciencefidelity.astro/) <span style="margin: 0.25em;"><Badge variant="neutral">دعم مجتمعي</Badge></span> - يوفر تلوين الكود، وإكمال الجمل على محرر Nova
- [مُلحق Vim](https://github.com/wuelnerdotexe/vim-astro) <span style="margin: 0.25em;"><Badge variant="neutral">دعم مجتمعي</Badge></span> - يوفر تلوين الكود، وطيه، ويدعم الإزاحة (indentation) على محررات Vim و Neovim
- ملحقات [LSP](https://github.com/neovim/nvim-lspconfig/blob/master/doc/server_configurations.md#astro) و [TreeSitter](https://github.com/virchau13/tree-sitter-astro) لـNeovim <span style="margin: 0.25em;"><Badge variant="neutral">دعم مجتمعي</Badge></span> - يوفر تلوين الكود، وتحليله، وتوفير دعم الإكمال التلقائي في محرر Neovim

### بيئات تطوير JetBrains

نود دعم [Webstorm IDE](https://www.jetbrains.com/webstorm/). لكنه لا يدعم التقنيات التي نستخدمها لإنشاء الإضافات (أسترو يستخدم language servers لبناء الإضافات)، وليس لدينا القدرة على انشاء وصيانة إضافة جديدة كليًا. صوّت [لدعم أسترو على JetBrains](https://youtrack.jetbrains.com/issue/WEB-52015/Astro-Language-Support)، تتبع تقدم التصويت، وابحث عن حلول من مجتمع JetBrains. 

مع ذلك بيئة [Fleet IDE](https://www.jetbrains.com/fleet/) القادمة من JetBrains _ستدعم_ التقنيات التي نستخدمها لانشاء الإضافات (language server)، وحينها ستعمل أدواتنا بدون أي مشاكل.

## المحررات في المتصفح

بالإضافة للمحررات المثبة على جهازك، أسترو يعمل بشكل جيد على المحررات السحابية (المحررات في المتصفح عموما)، ويشمل الدعم:

- [StackBlitz](https://stackblitz.com/) و [CodeSandbox](https://codesandbox.io/) - محررات سحابية تعمل من المتصفح، تدعم تلوين الكود لملفات `.astro` بدون اِعداد
- [GitHub.dev](https://github.dev/) - يسمح بتثبيت إضافة Astro VS Code [كملحق web](https://code.visualstudio.com/api/extension-guides/web-extensions), ليوفر بعض مزايا الإضافة, حاليا يوفر تلوين الكود فقط.
- [Gitpod](https://gitpod.io/) - بيئة تطوير سحابية كاملة يمكنها تثبيت إضافة Astro VS Code الرسمية من OpenVSX.

## أدوات أخرى

### ESLint

[ESLint](https://eslint.org/) أشهر أدوات اكتشاف الاخطاء في الشفرة البرمجية لـ JavaScript و JSX. يمكن تثبيت [ملحق يوفره المجتمع](https://github.com/ota-meshi/eslint-plugin-astro) لدعم أسترو أيضا.

راجع [دليل المستخدم](https://ota-meshi.github.io/eslint-plugin-astro/user-guide/) لمعرفة المزيد حول تثبيت وإعداد ESLint لمشروعك.

### Prettier

[Prettier](https://prettier.io/) هو [منسق](https://ar.wikipedia.org/wiki/برتي_برنت) شائع لأكواد JavaScript, HTML, CSS وغيرها. لدعم تجميل أكواد أسترو، استخدم [ملحق Astro الرسمي لـ Prettier](https://github.com/withastro/prettier-plugin-astro).

للبدأ، ثبّت Prettier أولا، ثم ملحق أسترو على Prettier:

```shell
npm install --save-dev prettier prettier-plugin-astro
```

يتعرف Prettier تلقائيا على ملحق أسترو عند تشغيله:

```shell
prettier --write .
```

راجع ملف README [لملحق أسترو على Prettier](https://github.com/withastro/prettier-plugin-astro/blob/main/README.md) لمزيد من المعلومات حول الخيارات المدعومة وكيفية إعداد Prettier داخل VS Code والمزيد.

:::caution[الاستخدام مع مدير الحزم pnpm]
نظرًا لوجود إشكال في Prettier ، فلن يتم اكتشاف ملحق أسترو تلقائيًا عند استخدام [pnpm](https://pnpm.io/). من أجل العثور على الملحق، يجب إضافة الخيار التالي عند تشغيل Prettier:

```shell
prettier --write --plugin-search-dir=. .
```

استخدام Prettier في VS Code يحتاج بعض الإعداد الإضافي. راجع ملف README للملحق.
:::
