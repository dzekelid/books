---
swagger: "2.0"
info:
  title: New York Times Best Seller List Names
  description: "The names service returns a list of Best Sellers list names. It includes
    in the response the type of list (weekly or monthly) and when it was first published
    and last published. Lists have been added and removed over time. For example the
    Food and Diet list was added in 2013 and the Children\u2019s Chapter Books list
    was removed in 2012. The response also includes the list_name_encoded which you
    use when calling the details service."
  termsOfService: https://developer.nytimes.com/tou
  version: 2.0.0
host: api.nytimes.com
basePath: /svc
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /books/v2/lists/names.{format}:
    get:
      summary: Best Seller List Names
      description: The names service returns a list of Best Sellers list names
      operationId: GET_lists-names-format
      parameters:
      - in: query
        name: api-key
        description: The API key
      - in: query
        name: format
        description: The format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - books
definitions:
  Article:
    properties:
      section:
        description: This is a default description.
        type: get
      subsection:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      abstract:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
      thumbnail_standard:
        description: This is a default description.
        type: get
      short_url:
        description: This is a default description.
        type: get
      byline:
        description: This is a default description.
        type: get
      item_type:
        description: This is a default description.
        type: get
      updated_date:
        description: This is a default description.
        type: get
  Doc:
    properties:
      web_url:
        description: This is a default description.
        type: get
      snippet:
        description: This is a default description.
        type: get
      lead_paragraph:
        description: This is a default description.
        type: get
      abstract:
        description: This is a default description.
        type: get
      print_page:
        description: This is a default description.
        type: get
      blog:
        description: This is a default description.
        type: get
      source:
        description: This is a default description.
        type: get
      headline:
        description: This is a default description.
        type: get
      keywords:
        description: This is a default description.
        type: get
      pub_date:
        description: This is a default description.
        type: get
  Event:
    properties:
      event_id:
        description: This is a default description.
        type: get
      event_schedule_id:
        description: This is a default description.
        type: get
      last_modified:
        description: This is a default description.
        type: get
      event_name:
        description: This is a default description.
        type: get
      event_detail_url:
        description: This is a default description.
        type: get
      web_description:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      film_rating:
        description: This is a default description.
        type: get
      critic_name:
        description: This is a default description.
        type: get
  ArticleWithCountType:
    properties:
      url:
        description: This is a default description.
        type: get
      count_type:
        description: This is a default description.
        type: get
      column:
        description: This is a default description.
        type: get
      section:
        description: This is a default description.
        type: get
      byline:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      abstract:
        description: This is a default description.
        type: get
      published_date:
        description: This is a default description.
        type: get
      source:
        description: This is a default description.
        type: get
      media:
        description: This is a default description.
        type: get
  Movie:
    properties:
      display_title:
        description: This is a default description.
        type: get
      mpaa_rating:
        description: This is a default description.
        type: get
      critics_pick:
        description: This is a default description.
        type: get
      byline:
        description: This is a default description.
        type: get
      headline:
        description: This is a default description.
        type: get
      summary_short:
        description: This is a default description.
        type: get
      publication_date:
        description: This is a default description.
        type: get
      opening_date:
        description: This is a default description.
        type: get
      date_updated:
        description: This is a default description.
        type: get
      link:
        description: This is a default description.
        type: get
  Critic:
    properties:
      display_name:
        description: This is a default description.
        type: get
      sort_name:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      bio:
        description: This is a default description.
        type: get
      seo_name:
        description: This is a default description.
        type: get
      multimedia:
        description: This is a default description.
        type: get
  Concept:
    properties:
      concept_id:
        description: This is a default description.
        type: get
      concept_name:
        description: This is a default description.
        type: get
      is_times_tag:
        description: This is a default description.
        type: get
      concept_status:
        description: This is a default description.
        type: get
      vernacular:
        description: This is a default description.
        type: get
      concept_type:
        description: This is a default description.
        type: get
      concept_created:
        description: This is a default description.
        type: get
      concept_updated:
        description: This is a default description.
        type: get
      taxonomy:
        description: This is a default description.
        type: get
      links:
        description: This is a default description.
        type: get
  ConceptRelation:
    properties:
      concept_id:
        description: This is a default description.
        type: get
      concept_name:
        description: This is a default description.
        type: get
      is_times_tag:
        description: This is a default description.
        type: get
      concept_status:
        description: This is a default description.
        type: get
      vernacular:
        description: This is a default description.
        type: get
      concept_type:
        description: This is a default description.
        type: get
      concept_created:
        description: This is a default description.
        type: get
      concept_updated:
        description: This is a default description.
        type: get
x-collection-name: New York Times
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---