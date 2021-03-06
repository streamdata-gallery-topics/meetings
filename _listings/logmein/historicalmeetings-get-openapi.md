---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToMeeting Historical meetings
  description: 'Get historical meetings for the currently authenticated organizer
    that started within the specified date/time range. Remark: Meetings which are
    still ongoing at the time of the request are NOT contained in the result array.'
  version: 1.0.0
host: api.getgo.com
basePath: /G2M/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{groupKey}/upcomingMeetings:
    get:
      summary: Upcoming meetings by group
      description: Get upcoming meetings for a specified group. This API call is only
        available to users with the admin role. This API call can be used only for
        groups with maximum 50 organizers.
      operationId: GroupsUpcomingMeetingsByGroupKeyGet
      x-api-path-slug: groupsgroupkeyupcomingmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: groupKey
      responses:
        200:
          description: OK
      tags:
      - Upcoming
      - Meetings
      - By
      - Group
  /historicalMeetings:
    get:
      summary: Historical meetings
      description: 'Get historical meetings for the currently authenticated organizer
        that started within the specified date/time range. Remark: Meetings which
        are still ongoing at the time of the request are NOT contained in the result
        array.'
      operationId: HistoricalMeetingsGet
      x-api-path-slug: historicalmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: endDate
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Meetings
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