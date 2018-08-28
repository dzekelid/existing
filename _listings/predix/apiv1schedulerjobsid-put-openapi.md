---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Runtime Update an existing scheduler job.
  version: 1.0.0
  description: Updates the scheduled job. The updated changes will be effective from
    the next scheduling of this job. To suspend a job, update the job with state value
    'Inactive'. To resume a job, update the job with state value 'Active'.
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/resource:
    post:
      summary: Creates a list of resources for the given zone. Existing resources
        will be updated with the provided values.
      description: Creates a list of resources for the given zone. existing resources
        will be updated with the provided values..
      operationId: appendResourcesUsingPOST
      x-api-path-slug: v1resource-post
      parameters:
      - in: body
        name: resources
        description: resources
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - List
      - Of
      - Resourcesthe
      - Given
      - Zone
      - ""
      - Existing
      - Resources
      - Will
      - Be
      - Updated
      - Provided
      - Values
  /v1/subject:
    post:
      summary: Creates a list of subjects. Existing subjects will be updated with
        the provided values.
      description: Creates a list of subjects. existing subjects will be updated with
        the provided values..
      operationId: appendsubjectsUsingPOST_1
      x-api-path-slug: v1subject-post
      parameters:
      - in: body
        name: subjects
        description: subjects
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - List
      - Of
      - Subjects
      - ""
      - Existing
      - Subjects
      - Will
      - Be
      - Updated
      - Provided
      - Values
  /api/v1/scheduler/jobs/{id}:
    put:
      summary: Update an existing scheduler job.
      description: Updates the scheduled job. The updated changes will be effective
        from the next scheduling of this job. To suspend a job, update the job with
        state value 'Inactive'. To resume a job, update the job with state value 'Active'.
      operationId: updateJob
      x-api-path-slug: apiv1schedulerjobsid-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: path
        name: id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: header
        name: Refresh-Token-For-Job-Execution
        description: Refresh-Token-For-Job-Execution
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Existing
      - Scheduler
      - Job
  /api/v2/config/orchestrations/{id}:
    put:
      summary: Update an existing orchestration configuration entry.
      description: Updates the orchestration configuration entry with given orchestration
        configuration.
      operationId: updateOrchestrationEntry
      x-api-path-slug: apiv2configorchestrationsid-put
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: body
        name: body
        description: orchestration configuration entry
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: orchestration configuration id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      responses:
        2:
          description: Successful response
      tags:
      - Existing
      - Orchestration
      - Configuration
      - Entry
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