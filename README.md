# Movie-Search
Movie search is used to check the movie related all information

Frontend:
Lightning Web Components (LWC) → your movieDetail component handles search input and displays results.
HTML template loops through movies and shows title, year, poster.
CSS for styling (cursor, layout, etc.).
Backend / API:
OMDb API → provides movie data.
Search endpoint: ?s=<title> returns a list with imdbID.
Detail endpoint: ?i=<imdbID>&plot=full returns full movie info.
Integration:
fetch() in LWC JS calls OMDb API.
Response JSON is parsed and bound to tracked properties (@track movies).
Errors handled via data.Response check.

Deployment Context:
Salesforce Org (Developer Edition).
Component exposed in movieDetail.js-meta.xml with targets like lightning__CommunityPage.
Available in Experience Builder → “Movie Search” workspace.
