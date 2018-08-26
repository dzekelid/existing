---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Parameters for editing existing audio widget on a layout
  description: Parameters for editing existing audio widget on a layout, for adding
    new audio, please refer to POST /library documentation
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /playlist/widget/audio/{playlistId}:
    post:
      summary: Parameters for editing existing audio widget on a layout
      description: Parameters for editing existing audio widget on a layout, for adding
        new audio, please refer to POST /library documentation
      operationId: WidgetAudioEdit
      x-api-path-slug: playlistwidgetaudioplaylistid-post
      parameters:
      - in: formData
        name: duration
        description: Edit Only - The Widget Duration
      - in: formData
        name: loop
        description: Edit only - Flag (0, 1) Should the audio loop (only for duration
          > 0 )?
      - in: formData
        name: mute
        description: Edit only - Flag (0, 1) Should the audio be muted?
      - in: formData
        name: name
        description: Edit Only - The Widget name
      - in: formData
        name: useDuration
        description: Edit Only - (0, 1) Select 1 only if you will provide duration
          parameter as well
      responses:
        200:
          description: OK
      tags:
      - Parametersediting
      - Existing
      - Audio
      - Widget
      - "On"
      - Layout
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