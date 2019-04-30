In this case:

```bash
GET / looks up the current list of uploaded files from the StorageService and loads it into a Thymeleaf template. It calculates a link to the actual resource using MvcUriComponentsBuilder
```
```bash
GET /files/{filename} loads the resource if it exists, and sends it to the browser to download using a "Content-Disposition" response header
```
```bash
POST / is geared to handle a multi-part message file and give it to the StorageService for saving
```
