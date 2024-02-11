--git branch -m main <BRANCH>
git fetch origin
git branch -u origin/<BRANCH> <BRANCH>
git remote set-head origin -a
**Additional context**
Add any other context about the problem here.https://console.vectara.com/console/corpora/createhttps://github.com/Hormigas-ai/Hormigas-ai-.git

// to use this install node-fetch from npm using 'npm install node-fetch --save'
fetch("https://api.vectara.io:443/v1/create-corpus", {
headers: {
  "Content-Type": "application/json",
  authorization: "Bearer eyJraWQiOiJvUnVNVmNrXC9DRFN2R2RDa2ViVEc2SVIwM0NCbmtlbnRISjFkNGFEZUZpUT0iLCJhbGciOiJSUzI1NiJ9.eyJhdF9oYXNoIjoiWGhfWjBqX1U4cGUxSDJzNElTek1PdyIsInN1YiI6IjI4MTRlNmZmLWZlZDQtNGVjMi1iNjA2LWYyZGNiZjMwNjU4NiIsImNvZ25pdG86Z3JvdXBzIjpbInVzLXdlc3QtMl9KMFZqQnd6b1dfR29vZ2xlIl0sImVtYWlsX3ZlcmlmaWVkIjp0cnVlLCJpc3MiOiJodHRwczpcL1wvY29nbml0by1pZHAudXMtd2VzdC0yLmFtYXpvbmF3cy5jb21cL3VzLXdlc3QtMl9KMFZqQnd6b1ciLCJjb2duaXRvOnVzZXJuYW1lIjoiR29vZ2xlXzExMTEwMTQ4NzI4MDUwOTU5NzY2OSIsImdpdmVuX25hbWUiOiJjcmlzd2FycmlvcnR2MzU0Iiwib3JpZ2luX2p0aSI6ImMyNWRiY2U5LWFhMDYtNDllZi1iMjljLWM1M2YyMzM2NDM3YiIsImF1ZCI6IjV1a2Y2djluOWI3bW9wcmVtaHAyOWMyc3RvIiwiaWRlbnRpdGllcyI6W3sidXNlcklkIjoiMTExMTAxNDg3MjgwNTA5NTk3NjY5IiwicHJvdmlkZXJOYW1lIjoiR29vZ2xlIiwicHJvdmlkZXJUeXBlIjoiR29vZ2xlIiwiaXNzdWVyIjpudWxsLCJwcmltYXJ5IjoidHJ1ZSIsImRhdGVDcmVhdGVkIjoiMTcwNzYxMjM0NDM4OSJ9XSwidG9rZW5fdXNlIjoiaWQiLCJhdXRoX3RpbWUiOjE3MDc2MTIzNDYsIm5hbWUiOiJjcmlzd2FycmlvcnR2MzU0IiwiZXhwIjoxNzA3NjI1OTMwLCJpYXQiOjE3MDc2MjIzMzEsImp0aSI6Ijk1YzM1NzM1LTVlMjUtNDUxZC05OWVkLTliM2NlNGQ1MmQxMiIsImVtYWlsIjoiY3Jpc3dhcnJpb3J0djJAZ21haWwuY29tIn0.qv6LcVJJ3K7eY7nYspryG_jbAhLHivGBzNZhekvwcKn9jjYnV6xJU-XkbdPWLxz8J7olNmH7NyWW7u6cQFR6-xJZlsBNwmUxzPnAt8qQzQekc1XDkfhMHgR4Oth3WVr7fkfreu9d3OFCCSKt8a6hKCAWuD8kOeWfftDSWTbu5DWuIZWnjLuSWU4Hc8w1pXiqtzvYx-n5ylfUgZymFanbk-FKdy-zeoB4KqWZnv7cjuLVH1jMhJ1psLZwc1qOgxpVJZ0EzVBoKsXSKnpQ4SYFoCDAOqczHQs0meQyCpFAhxX51h8AohlxJDu3xwhuXev5Wlgm-x24iXZZxOSkWexsqQ",
  "customer-id": "910181580",
},
body: "{\"corpus\":{\"id\":0,\"name\":\"\",\"description\":\"\",\"dtProvision\":0,\"enabled\":false,\"swapQenc\":false,\"swapIenc\":false,\"textless\":false,\"encrypted\":true,\"encoderId\":0,\"metadataMaxBytes\":0,\"faissIndexType\":\"\",\"customDimensions\":[],\"filterAttributes\":[{\"name\":\"lang\",\"description\":\"Detected language, as an ISO 639-3 code.\",\"indexed\":true,\"type\":25,\"level\":10},{\"name\":\"is_title\",\"description\":\"True if the text is a title.\",\"indexed\":true,\"type\":35,\"level\":10}]}}",
method: "post",
})
.then((res) => res.json())
.then((data) => console.log(data))
.catch((error) => console.log(error))
        