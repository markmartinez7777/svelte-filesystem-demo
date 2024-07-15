# Svelte Filesystem Proof of concept

This is Quick POC of [an idea i had](https://twitter.com/swyx/status/1396005314227539968): what if you could edit Svelte components in place in the browser — using the File System Access API!

What if we didn't have to mentally map our source code rendered content? Just click on component, source pops up, we edit, save. **No IDE needed!**

> note: this idea works only in development - which makes sense if you think about it


https://user-images.githubusercontent.com/6764957/120790682-d9b7c400-c565-11eb-9580-740279005543.mp4


[see tweet responses](https://twitter.com/swyx/status/1400764771520040963)

## usage

```bash
npm install
npm run dev -- --open # localhost 
```

- Click `load` button to open `src/components/Comp.svelte` - you will have to navigate there yourself until [this PR lands](https://github.com/WICG/file-system-access/pull/287)
- try making edits the source
- then hit the `save` button
- see it hot reload thanks to Vite/SvelteKit. 

You now have a self-editing component!
