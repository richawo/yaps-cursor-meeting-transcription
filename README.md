# Yaps Meeting Notes

Turn recordings into speaker-labelled meeting notes, recaps, chapters, and grounded answers with the local Yaps engine.

One purpose-specific Cursor plugin, with one skill and one local MCP server. Install only the Yaps workflows you need. All twelve packages use the same maintained runtime and the models already installed in Yaps.

## Setup

1. Install [Yaps desktop](https://yaps.ai/download) on this computer and sign in with active desktop access.
2. Install Node.js 20+ with npm/npx. First launch downloads a small helper package and its JavaScript dependencies from the npm registry. Git and a source checkout are not required.
3. Add this repository as a Cursor plugin, or use its Cursor Directory components. A directory MCP install button installs the server configuration; add the skill separately when using that component flow.
4. Use yaps_status to check readiness. Missing feature models can be installed after your agreement; existing models and your Yaps account are reused.

The runtime is pinned to [yaps-cursor-runtime@0.3.0](https://www.npmjs.com/package/yaps-cursor-runtime/v/0.3.0). There are no API keys to supply. Yaps handles local processing and feature model downloads. Yaps 2.3.124 is only the credential-free account-check floor; this workflow requires 2.3.848 or newer.

## Scope and validation

This is a local Cursor integration. Grok Bot runs primarily in the cloud; its local-execution integration and marketplace distribution have not been validated. Do not treat this package as an automatic Grok Bot listing.

The shared runtime has direct macOS MCP and Auto Cut export coverage. Windows and live host UI validation must be reported separately; a listing approval does not prove those paths. Model-download code is present, but a fresh download has not been exercised for every workflow.

## Maintenance

Generated from [the central catalog](https://github.com/richawo/yaps-plugins/blob/main/cursor/standalone-plugins.json) and its skill sources. Update the central runtime and catalog, validate, then regenerate using scripts/generate-cursor-standalone.mjs. Do not copy or fork the helper into this repository. Keep directory-component.json's named wrapper when updating a directory install payload.

[Privacy](https://yaps.ai/privacy) · [Terms](https://yaps.ai/terms) · MIT license
