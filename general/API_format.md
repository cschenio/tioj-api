API Format
==========

The API would be categorized and described in the following format:

**HTTP-VERB** {Domain-name}/{Version}/{Noun}.{format} _(Entire Collection)_

or

**HTTP-VERB** {Domain-name}/{Version}/{Noun}/{:id}.{format} _(Specific Item)_

## HTTP-VERB
  There are four verbs in this release, combining with two types of endpoint above:

  + POST: 
    - {Noun}: to create something in the collection.
    - {Noun}/{:id}: invalid.
  + GET:
    - {Noun}: to grab the whole collection at one time.
    - {Noun}/{:id}: to retrieve the certain item.
  + PATCH: 
    - {Noun}: invalid.
    - {Noun}/{:id}: to (partially) update something.
  + DELETE:
    - {Noun}: invalid due to the danger.
    - {Noun}/{:id}: to delete something.

## Domain-name 
  We highly suggested that one should use either _api.abc.xyz/_ or _abc.xyz/api/_ as one's domain name in order to point out the type of the response.

## Version 
  In this release, we use "v1" as the api version.

## Noun 
  We **always** use plural noun for the responses involve resources. 

## Id
  The id is usually a serial integer, which represents to certain problem or submission. But it might also be string like the cases of username.

## Format
  The server-side should at least provide the following formats for the client-side to fetch:
  + xml
  + json
  + yaml

## Examples

### Available Format
  - GET www.johncena.com/api/v1/dogs/3.json _(Typical)_
  - GET api.whyrusoloud.net/v1/cats/1.csv _(Provide something more than basic format)_
  - PATCH api.youthexcited.com/v1/people/meijiang.json _(Id need not be integer)_
  - POST www.letmeseesee.org/v1/mice.xml _(Though no "api" in the domain name, it is still available)_

### Unavailable Format
  - GET lovelife.com/api/v1.0/dances/1.json _(Wrong version number)_
  - PATCH raburaibu.com/api/v1/song.yaml _(Wrong plurality)_
  - POST api.sukiyaki.org/v1/pots/2.xml _(Invalid HTTP Verb)_