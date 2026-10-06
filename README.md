# Co-Centre tools website

Source for https://foodcocentre.github.io, the index of computational tools
produced by the Co-Centre for Sustainable Food Systems.

The site is built with [Jekyll](https://jekyllrb.com/) and published
automatically by GitHub Pages whenever changes are committed to `main`.

## Adding your tool

1. Make sure your tool has a **licence**, a **README**, and a tagged
   **release** (e.g. `v1.0.0`) in its repository.
2. Edit [`_data/tools.yml`](_data/tools.yml) and add an entry at the end:

```yaml
   - name: My Tool
     description: One or two sentences on what it does.
     maintainer: Your Name
     stable_version: v1.0.0
     stable_repo: https://github.com/foodcocentre/my-tool
     latest_repo: https://github.com/your-username/my-tool
     app_url:
     doi:
```

3. Commit the change. The site rebuilds within a couple of minutes.

If you're not yet a member of the organisation, contact James to be added or fork this repo and open a pull
request instead.

### Field guide

| Field | Meaning |
|---|---|
| `name` | Display name of the tool |
| `description` | Short summary (1-2 sentences) |
| `maintainer` | Person to contact about the tool |
| `stable_version` | Version number of the deposited release |
| `stable_repo` | Repo in this organisation holding the stable release |
| `latest_repo` | Where development continues (often a personal repo) |
| `app_url` | Optional link to a hosted app |
| `doi` | Optional DOI (e.g. from Zenodo), without `https://doi.org/` |

Leave optional fields blank rather than deleting them. Keep the indentation
exactly as shown, because YAML is sensitive to spaces.

## Stable versions and ownership

We encourage researchers to transfer finished tools to this organisation and
fork them back to their own account for continued development. The website
shows both: the stable Co-Centre copy and the latest development version.

## Contact

James Gillespie (j.gillespie@qub.ac.uk)
