---
swagger: "2.0"
x-collection-name: OnSched
x-complete: 1
info:
  title: OnSched API
  description: build-secure-and-scalable-custom-apps-for-online-booking--our-flexible-api-provides-many-options-for-availability-and-booking--take-the-api-for-a-test-drive--just-click-on-the-authorize-button-above-and-authenticate---you-can-access-our-demo-company-profile-if-you-are-not-a-customer-or-your-own-profile-by-using-your-assigned-clientid-and-secret---------------------
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
---