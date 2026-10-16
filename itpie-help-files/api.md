# API

Source: ITPIE:OPS Documentation — API
Source URL: https://itpie-hostname/documentation/content/api.html
Document set: itpie-help-files
Citation rule: every line below begins with the documentation page title and its URL. When answering from this document, always name the page title and link.

## Content

[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] API
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] The application provides an HTTP API (sometimes called a REST API).
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] Authentication
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] The API requires authentication with an access token, which you can create by following the instructions on Settings > Preferences . You should use an Authorization header with the Bearer scheme.
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] For example:
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] cURL
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] Python
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] curl -H "Authorization: Bearer <ACCESS_TOKEN>" https://www.example.com/api/search/device?term=*
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] using System; using System.Net; using System.Net.Http; using System.Net.Http.Headers; var client = new HttpClient(); client.DefaultRequestHeaders.Accept.Clear(); client.DefaultRequestHeaders.Accept.Add(new MediaTypeWithQualityHeaderValue("application/json")); client.DefaultRequestHeaders.Authorization = new AuthenticationHeaderValue("Bearer", "<ACCESS_TOKEN>"); var response = await client.GetAsync("https://example.com/api/search/device?term=*"); response.EnsureSuccessStatusCode(); var content = await response.Content.ReadAsStringAsync(); Console.WriteLine(content);
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] import requests headers = {"Authorization": "Bearer <ACCESS_TOKEN>"} response = requests.get("https://example.com/api/search/device?term=*", headers=headers, verify=False) print(response.json())
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] OpenAPI
[ITPIE:OPS Documentation | API | https://itpie-hostname/documentation/content/api.html] OpenAPI 3.0 swagger json is available upon request. Please contact your ITPIE Technical Support to get a copy of the specification.