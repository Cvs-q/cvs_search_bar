# CVS Search Bar

Small Frappe app that puts a v15-style search bar at the top right of the Frappe v16 desk.
It is kept separate from `cvs_internal_improvements` so it can be tested and updated on its own.

| File | Purpose |
|---|---|
| `cvs_search_bar/public/js/search_top_right.js` | Adds the search button and opens Frappe's search |
| `cvs_search_bar/public/css/search_top_right.css` | Position and look of the bar |
| `cvs_search_bar/hooks.py` | Loads the JS and CSS on every desk page (`app_include_js`, `app_include_css`) |

## Install

```
bench get-app <repo-url>
bench --site <site> install-app cvs_search_bar
bench build --app cvs_search_bar
```
