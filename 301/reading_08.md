# Reading 8

## API Best Design Practices [Link](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

**REST**: Respresentational State Transfer

REST APIs are:
- Designed around resources
- Driven by hypermedia links
- Use a stateless request model

### What is an identifer of a resource? Give an example.

An identifier is unique to the resource. For example, an isbn number for a resource like a book. 

**HTTP verbs**: GET, POST, PUT, PATCH, DELETE
These are standard and included in the uniform interface for REST APIs that are built using HTTP.

**URIs** should be based on nouns and NOT verbs. Meaning, something like `https://github.com/profile` is better than `https://github.com/edit-profile`

A good URI also doesn't have the exact same wording as what is going on internally in the program- it is good to make the client unaware of that terminology

It is also good form to have a naming convention for URI.

*A ‘chatty’ web API?* means that the API is sending a bunch of requests for individual or small chunks of data. It is better to request this data is fewer requests.

- **Get** gets the representation of a resource at the URI
- **Post** creates new resource at URI, or can trigger operations that don't create resources
- **Put** takes the resource at the URI and replaces or creates it
- **Patch** does a partial update of resource
- **Delete** removes resource at URI

- a successful GET request returns --> 202 (OK)
- an unsuccessful GET request returns --> 404 (Not Found)
- a successful POST or PUT request returns --> 201 (Created)
- a successful DELETE request returns --> 204




[Home](https://peymade.github.io/reading-notes/)