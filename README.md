# Trade Portal policies

The Terms of Service and Privacy Policy for [tradeportal.pro](https://secure.tradeportal.pro),
published with GitHub Pages.

## Editing

Every company-specific fact lives in `_config.yml` and is referenced from the
documents as `{{ site.whatever }}`. Change it there, not in the legal text.

Three values are still `TODO` and render literally on the published page until
they are filled in — deliberately, because a visibly wrong placeholder is safer
in a legal document than a plausible guess:

- `legal_entity` — registered company name and number
- `company_address` — registered office
- `jurisdiction` — governing law

The subprocessor table in `privacy/index.md` was compiled from the integrations
present in the application code, not from a contract inventory. Confirm it before
publishing: GDPR Article 28 requires it to be accurate and current.

## Publishing

Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/`.
GitHub builds the Jekyll site itself; there is no workflow and no Gemfile to keep
in step. The layout in `_layouts/default.html` is self-contained — no theme gem,
no webfont, nothing fetched from a third party on a page about privacy.

To preview locally: `jekyll build` or `jekyll serve`.

## Unadapted documents

The upstream repository also carries cancellation, refund, use restrictions,
security, taxes, SLA and product-ownership policies. Those files are still here
but are **not linked** from the index and still describe Basecamp and HEY. Adapt
them before linking, or delete them.

## Licence

Adapted from the [37signals open-source policies](https://github.com/basecamp/policies),
used under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Changes have
been made. Attribution in the page footer is a licence condition — keep it.
