In this case:

```bash
GET / 

Looks up the current list of uploaded files from the StorageService and loads it into a Thymeleaf template. It calculates a link to the actual resource using MvcUriComponentsBuilder
```
```bash
GET /files/{filename} 

Loads the resource if it exists, and sends it to the browser to download using a "Content-Disposition" response header
```
```bash
POST / 

Geared to handle a multi-part message file and give it to the StorageService for saving
```
