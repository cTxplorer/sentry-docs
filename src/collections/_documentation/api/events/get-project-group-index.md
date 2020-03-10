---
# This file is automatically generated from the API using `sentry/api-docs/generator.py.`
# Do not manually edit this file.
{
  "api_path": "/api/0/projects/{organization_slug}/{project_slug}/issues/", 
  "authentication": "required", 
  "description": "Return a list of issues (groups) bound to a project.  All parameters are\nsupplied as query string parameters.\n\nA default query of ``is:unresolved`` is applied. To return results\nwith other statuses send an new query value (i.e. ``?query=`` for all\nresults).\n\nThe ``statsPeriod`` parameter can be used to select the timeline\nstats which should be present. Possible values are: ``\"\"`` (disable),\n``\"24h\"``, ``\"14d\"``", 
  "example_request": "GET /api/0/projects/the-interstellar-jurisdiction/pump-station/issues/?statsPeriod=24h HTTP/1.1\nHost: sentry.io\nAuthorization: Bearer <token>", 
  "example_response": "HTTP/1.1 200 OK\nContent-Length: 2326\nX-XSS-Protection: 1; mode=block\nContent-Language: en\nX-Max-Hits: 1000\nAccess-Control-Expose-Headers: X-Sentry-Error, Retry-After\nVary: Accept-Language, Cookie\nX-Content-Type-Options: nosniff\nAccess-Control-Allow-Methods: GET, PUT, DELETE, HEAD, OPTIONS\nLink: <https://sentry.io/api/0/projects/the-interstellar-jurisdiction/pump-station/issues/?statsPeriod=24h&cursor=1583819858583:0:1>; rel=\"previous\"; results=\"false\"; cursor=\"1583819858583:0:1\", <https://sentry.io/api/0/projects/the-interstellar-jurisdiction/pump-station/issues/?statsPeriod=24h&cursor=1583819856132:1:0>; rel=\"next\"; results=\"false\"; cursor=\"1583819856132:1:0\"\nX-Hits: 2\nAllow: GET, PUT, DELETE, HEAD, OPTIONS\nAccess-Control-Allow-Origin: *\nAccess-Control-Allow-Headers: X-Sentry-Auth, X-Requested-With, Origin, Accept, Content-Type, Authentication, Authorization\nContent-Type: application/json\nX-Frame-Options: deny\n\n[\n  {\n    \"annotations\": [], \n    \"assignedTo\": null, \n    \"count\": \"1\", \n    \"culprit\": \"io.sentry.example.ApiRequest in perform\", \n    \"firstSeen\": \"2020-03-10T05:57:38.583871Z\", \n    \"hasSeen\": false, \n    \"id\": \"2\", \n    \"isBookmarked\": false, \n    \"isPublic\": false, \n    \"isSubscribed\": false, \n    \"lastSeen\": \"2020-03-10T05:57:38.583871Z\", \n    \"level\": \"error\", \n    \"logger\": null, \n    \"metadata\": {\n      \"filename\": \"ApiRequest.java\", \n      \"function\": \"perform\", \n      \"type\": \"ApiException\", \n      \"value\": \"Authentication failed, token expired!\"\n    }, \n    \"numComments\": 0, \n    \"permalink\": \"https://sentry.io/organizations/the-interstellar-jurisdiction/issues/2/\", \n    \"platform\": \"java\", \n    \"project\": {\n      \"id\": \"2\", \n      \"name\": \"Pump Station\", \n      \"platform\": null, \n      \"slug\": \"pump-station\"\n    }, \n    \"shareId\": null, \n    \"shortId\": \"PUMP-STATION-2\", \n    \"stats\": {\n      \"24h\": [\n        [\n          1583733600, \n          0\n        ], \n        [\n          1583737200, \n          0\n        ], \n        [\n          1583740800, \n          0\n        ], \n        [\n          1583744400, \n          0\n        ], \n        [\n          1583748000, \n          0\n        ], \n        [\n          1583751600, \n          0\n        ], \n        [\n          1583755200, \n          0\n        ], \n        [\n          1583758800, \n          0\n        ], \n        [\n          1583762400, \n          0\n        ], \n        [\n          1583766000, \n          0\n        ], \n        [\n          1583769600, \n          0\n        ], \n        [\n          1583773200, \n          0\n        ], \n        [\n          1583776800, \n          0\n        ], \n        [\n          1583780400, \n          0\n        ], \n        [\n          1583784000, \n          0\n        ], \n        [\n          1583787600, \n          0\n        ], \n        [\n          1583791200, \n          0\n        ], \n        [\n          1583794800, \n          0\n        ], \n        [\n          1583798400, \n          0\n        ], \n        [\n          1583802000, \n          0\n        ], \n        [\n          1583805600, \n          0\n        ], \n        [\n          1583809200, \n          0\n        ], \n        [\n          1583812800, \n          0\n        ], \n        [\n          1583816400, \n          1\n        ]\n      ]\n    }, \n    \"status\": \"unresolved\", \n    \"statusDetails\": {}, \n    \"subscriptionDetails\": null, \n    \"title\": \"ApiException: Authentication failed, token expired!\", \n    \"type\": \"error\", \n    \"userCount\": 1\n  }, \n  {\n    \"annotations\": [], \n    \"assignedTo\": null, \n    \"count\": \"1\", \n    \"culprit\": \"raven.scripts.runner in main\", \n    \"firstSeen\": \"2020-03-10T05:57:36.131694Z\", \n    \"hasSeen\": false, \n    \"id\": \"1\", \n    \"isBookmarked\": false, \n    \"isPublic\": false, \n    \"isSubscribed\": false, \n    \"lastSeen\": \"2020-03-10T05:57:36.131694Z\", \n    \"level\": \"error\", \n    \"logger\": null, \n    \"metadata\": {\n      \"title\": \"This is an example python exception\"\n    }, \n    \"numComments\": 0, \n    \"permalink\": \"https://sentry.io/organizations/the-interstellar-jurisdiction/issues/1/\", \n    \"platform\": \"python\", \n    \"project\": {\n      \"id\": \"2\", \n      \"name\": \"Pump Station\", \n      \"platform\": null, \n      \"slug\": \"pump-station\"\n    }, \n    \"shareId\": null, \n    \"shortId\": \"PUMP-STATION-1\", \n    \"stats\": {\n      \"24h\": [\n        [\n          1583733600, \n          0\n        ], \n        [\n          1583737200, \n          0\n        ], \n        [\n          1583740800, \n          0\n        ], \n        [\n          1583744400, \n          0\n        ], \n        [\n          1583748000, \n          0\n        ], \n        [\n          1583751600, \n          0\n        ], \n        [\n          1583755200, \n          0\n        ], \n        [\n          1583758800, \n          0\n        ], \n        [\n          1583762400, \n          0\n        ], \n        [\n          1583766000, \n          0\n        ], \n        [\n          1583769600, \n          0\n        ], \n        [\n          1583773200, \n          0\n        ], \n        [\n          1583776800, \n          0\n        ], \n        [\n          1583780400, \n          0\n        ], \n        [\n          1583784000, \n          0\n        ], \n        [\n          1583787600, \n          0\n        ], \n        [\n          1583791200, \n          0\n        ], \n        [\n          1583794800, \n          0\n        ], \n        [\n          1583798400, \n          0\n        ], \n        [\n          1583802000, \n          0\n        ], \n        [\n          1583805600, \n          0\n        ], \n        [\n          1583809200, \n          0\n        ], \n        [\n          1583812800, \n          0\n        ], \n        [\n          1583816400, \n          1\n        ]\n      ]\n    }, \n    \"status\": \"unresolved\", \n    \"statusDetails\": {}, \n    \"subscriptionDetails\": null, \n    \"title\": \"This is an example python exception\", \n    \"type\": \"default\", \n    \"userCount\": 1\n  }\n]", 
  "method": "GET", 
  "parameters": null, 
  "path_parameters": [
    {
      "description": "the slug of the organization the issues belong to.", 
      "name": "organization_slug", 
      "type": "string"
    }, 
    {
      "description": "the slug of the project the issues belong to.", 
      "name": "project_slug", 
      "type": "string"
    }
  ], 
  "query_parameters": [
    {
      "description": "an optional stat period (can be one of `\"24h\"`, `\"14d\"`, and `\"\"`).", 
      "name": "statsPeriod", 
      "type": "string"
    }, 
    {
      "description": "if this is set to true then short IDs are looked up by this function as well.  This can cause the return value of the function to return an event issue of a different project which is why this is an opt-in. Set to 1 to enable.", 
      "name": "shortIdLookup", 
      "type": "bool"
    }, 
    {
      "description": "an optional Sentry structured search query.  If not provided an implied `\"is:unresolved\"` is assumed.)", 
      "name": "query", 
      "type": "querystring"
    }, 
    {
      "description": "this restricts the issues to ones containing events from this environment", 
      "name": "environment", 
      "type": "string"
    }
  ], 
  "sidebar_order": 12, 
  "title": "List a Project's Issues", 
  "warning": null
}
---