Reproduction of Storybook multiple `preview.ts` loading when imported issue.

Repro:

1. Start storybook
2. Visit, with console open
3. Notice `preview.ts loaded` is logged twice.
4. Comment out https://github.com/tmeasday/storybook-preview-import/blob/5066b694865d8bcb75400d2c0afc4498a6a1c327/src/stories/Button.stories.ts#L3
5. Reload
6. Notice `preview.ts loaded` is logged once (correct behaviour).
