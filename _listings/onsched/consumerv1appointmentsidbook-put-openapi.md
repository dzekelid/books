---
swagger: "2.0"
x-collection-name: OnSched
x-complete: 0
info:
  title: OnSched Returns an appointment object
  description: "This end point completes a new booking. Only appointments in the \"IN\"
    initial status can be booked.\r\nby saving all the relevant details of the booking.\r\n\r\nA
    valid appointment id is required. Use the appointmentId returned from POST /consumer/v1/appointments\r\n\r\nTo
    update appointment custom field values, use the GET /consumer/v1/appointments/customfields
    information\r\nto understand your definitions of custom fields and what key and
    values to update."
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/appointments/{id}/book:
    put:
      summary: Returns an appointment object
      description: "This end point completes a new booking. Only appointments in the
        \"IN\" initial status can be booked.\r\nby saving all the relevant details
        of the booking.\r\n\r\nA valid appointment id is required. Use the appointmentId
        returned from POST /consumer/v1/appointments\r\n\r\nTo update appointment
        custom field values, use the GET /consumer/v1/appointments/customfields information\r\nto
        understand your definitions of custom fields and what key and values to update."
      operationId: ConsumerV1AppointmentsByIdBookPut
      x-api-path-slug: consumerv1appointmentsidbook-put
      parameters:
      - in: body
        name: appointmentBookModel
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Appointments
      - Book
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