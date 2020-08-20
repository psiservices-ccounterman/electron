# PostBody Object

* `data` Array<[PostData](./post-data.md)> - The post data to be sent to the
  new window.
* `contentType` String - The `content-type` header used for the data. One of
  `application/x-www-form-urlencoded` or `multipart/form-data`. Corresponds to
  the `enctype` attribute of the submitted HTML form.
* `boundary` String (optional) - The boundary used to separate multiple parts of
  the message. Only valid when `contentType` is `multipart/form-data`.
