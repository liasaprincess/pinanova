<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

## Project architecture
- Keep shared website navigation and footer in a reusable SiteShell rendered by the root route; each content page owns its metadata.
- Keep contact validation in a shared schema and writes in a public server function with handler-only privileged imports; submissions are private and owner-readable through Cloud.
- Treat collection imagery as editorial previews, not purchasable inventory, until a real catalog is supplied.
