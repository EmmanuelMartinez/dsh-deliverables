# dsh-deliverables-minimal

A minimal header for the changed-files card in the DeepSeek Harness Web/Desktop
client, replacing the in-box \`ui-deliverables\` card.

The card keeps its rows, hover preview, and review opener; the header loses the
40px icon tile and the two-line title block, so the icon, the title, and the
added/deleted counts sit on one 34px row.

## Install

In the DeepSeek Harness Desktop Plugin Manager choose **Add plugin** and enter:

\`\`\`
github:EmmanuelMartinez/dsh-deliverables#v1.0.0
\`\`\`

Then restart the application. The card is replaced on the next turn that edits
files. Plugins do not auto-update: uninstall and reinstall to move versions.

## What the patch does

The bundle's \`cordis.patch.yml\` disables the deployment's own
\`ui-deliverables\` row and inserts this package's row, so the browser half
served for the card is this one. The package ships the same Host half, so
file-reference guidance and authenticated native opens are unchanged.
