# Read-07
#### Teams prefering
Imagine you have been invited to join one of two groups.

Team A is composed of people who are all exceptionally smart and successful. When you watch a video of this group working, you see professionals who wait until a topic arises in which they are expert, and then they speak at length, explaining what the group ought to do. When someone makes a side comment, the speaker stops, reminds everyone of the agenda and pushes the meeting back on track. This team is efficient. There is no idle chitchat or long debates. The meeting ends as scheduled and disbands so everyone can get back to their desks.

Team B is different. It’s evenly divided between successful executives and middle managers with few professional accomplishments. Teammates jump in and out of discussions. People interject and complete one another’s thoughts. When a team member abruptly changes the topic, the rest of the group follows him off the agenda. At the end of the meeting, the meeting doesn’t actually end: Everyone sits around to gossip and talk about their lives.

***Which group would you rather join?***
‘‘Over the past century, psychologists made considerable progress in defining and systematically measuring intelligence in individuals,’’ the researchers wrote in the journal Science in 2010. ‘‘We have used the statistical approach they developed for individual intelligence to systematically measure the intelligence of groups.’’ 

#### SuperAgent
SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!

#### GET requests
The .query() method accepts objects, which when used with the GET method will form a query-string.
#### HEAD requests
You can also use the .query() method for HEAD requests.
#### POST / PUT requests
A typical JSON POST request might look a little like the following, where we set the Content-Type header field appropriately, and "write" some data, in this case just a JSON string.
#### Setting the Content-Type
```
 request.post('/user')
   .set('Content-Type', 'application/json')
   ```

   As a short-hand the .type() method is also available, accepting the canonicalized MIME type name complete with type/subtype, or simply the extension name

   ``` 
    request.post('/user')
   .type('application/json')

 request.post('/user')
   .type('json')

 request.post('/user')
   .type('png')
   ```
   #### Retrying requests
   When given the .retry() method, SuperAgent will automatically retry requests, if they fail in a way that is transient or could be due to a flaky Internet connection.
   ```
    request
   .get('https://example.com/search')
   .retry(2) // or:
   .retry(2, callback)
   .then(finished);
   .catch(failed);
   ```
   Use .retry() only with requests that are idempotent ( multiple requests reaching the server won't cause undesirable side effects like duplicate purchases).
   #### Setting Accept
   In a similar fashion to the `.type()` method it is also possible to set the Accept header via the short hand method `.accept()`.

   #### APIs
   * An API is a set of definitions and protocols for building and integrating application software.
   * APIs simplify how developers integrate new application components into an existing architectur
   * Public APIs represent unique business value because they can simplify and expand how you connect with your partners

   #### Approaches to API
   1. Private: The API is only for use internally.
   1. Partner: The API is shared with specific business partners.
   1. Public: The API is available to everyone.
   