---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToMeeting Meeting
  description: "Create a new meeting based on the parameters specified.\r\n\r\n\t\t\t\t\t\t\t\t\t\t\r\n\t\tfield\t\t\tvalue\t\t\tdescription\t\t\r\n\t\t\"subject\"\t\t\t\"subject\"\t\t\tString
    - max 100 char.\t\t\r\n\t\t\"starttime\"\t\t\t\"2019-05-10T12:00:00Z\"\t\t\t{YYYY}-{MM}-{DD}T{HH}:{MM}:{SS}Z
    format, UTC only\t\t\r\n\t\t\"endtime\"\t\t\t\"2019-05-10T13:00:00Z\"\t\t\t{YYYY}-{MM}-{DD}T{HH}:{MM}:{SS}Z
    format, UTC only\t\t\r\n\t\t\"passwordRequired\"\t\t\tFALSE\t\t\tBoolean: true,
    false\t\t\r\n\t\t\"conferencecallinfo\"\t\t\t\"hybrid\"\t\t\tMust be one of: Hybrid,
    PTSN, Free, Private, VoIP.\t\t\r\n\t\t\"timezonekey\"\t\t\t\t\t\tAll times default
    to UTC\t\t\r\n\t\t\"meetingtype\"\t\t\t\"scheduled\"\t\t\tMust be one of: scheduled,
    recurring, immediate"
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
  /upcomingMeetings:
    get:
      summary: Upcoming meetings
      description: Gets upcoming meetings for the current authenticated organizer.
      operationId: UpcomingMeetingsGet
      x-api-path-slug: upcomingmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Upcoming
      - Meetings
  /organizers/{organizerKey}/historicalMeetings:
    get:
      summary: Historical meetings by organizer
      description: Get historical meetings for the specified organizer that started
        within the specified date/time range. Meetings which are still ongoing at
        the time of the request are not included in the result.
      operationId: OrganizersHistoricalMeetingsByOrganizerKeyGet
      x-api-path-slug: organizersorganizerkeyhistoricalmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: endDate
      - in: path
        name: organizerKey
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Meetings
      - By
      - Organizer
  /groups/{groupkey}/historicalMeetings:
    get:
      summary: Historical meetings by group
      description: 'Get historical meetings for the specified group that started within
        the specified date/time range. This API call is only available to users with
        the admin role. This API call is restricted to groups with a maximum of 50
        organizers. Remark: Meetings which are still ongoing at the time of the request
        are NOT contained in the result array.'
      operationId: GroupsHistoricalMeetingsByGroupkeyGet
      x-api-path-slug: groupsgroupkeyhistoricalmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: endDate
      - in: path
        name: groupkey
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Meetings
      - By
      - Group
  /meetings:
    post:
      summary: Meeting
      description: "Create a new meeting based on the parameters specified.\r\n\r\n\t\t\t\t\t\t\t\t\t\t\r\n\t\tfield\t\t\tvalue\t\t\tdescription\t\t\r\n\t\t\"subject\"\t\t\t\"subject\"\t\t\tString
        - max 100 char.\t\t\r\n\t\t\"starttime\"\t\t\t\"2019-05-10T12:00:00Z\"\t\t\t{YYYY}-{MM}-{DD}T{HH}:{MM}:{SS}Z
        format, UTC only\t\t\r\n\t\t\"endtime\"\t\t\t\"2019-05-10T13:00:00Z\"\t\t\t{YYYY}-{MM}-{DD}T{HH}:{MM}:{SS}Z
        format, UTC only\t\t\r\n\t\t\"passwordRequired\"\t\t\tFALSE\t\t\tBoolean:
        true, false\t\t\r\n\t\t\"conferencecallinfo\"\t\t\t\"hybrid\"\t\t\tMust be
        one of: Hybrid, PTSN, Free, Private, VoIP.\t\t\r\n\t\t\"timezonekey\"\t\t\t\t\t\tAll
        times default to UTC\t\t\r\n\t\t\"meetingtype\"\t\t\t\"scheduled\"\t\t\tMust
        be one of: scheduled, recurring, immediate"
      operationId: MeetingsPost
      x-api-path-slug: meetings-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Meeting
  /meetings/{meetingInstanceKey}/attendees:
    get:
      summary: Attendees by meeting
      description: List all attendees for specified meetingId of historical meeting.
        The historical meetings can be fetched using 'Get historical meetings', 'Get
        historical meetings by organizer', and 'Get historical meetings by group'.
        For users with the admin role this call returns attendees for any meeting.
        For any other user the call will return attendees for meetings on which the
        user is a valid organizer.
      operationId: MeetingsAttendeesByMeetingInstanceKeyGet
      x-api-path-slug: meetingsmeetinginstancekeyattendees-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: meetingInstanceKey
      responses:
        200:
          description: OK
      tags:
      - Attendees
      - By
      - Meeting
  /meetings/{meetingId}/start:
    get:
      summary: Meeting link
      description: Returns a host URL that can be used to start a meeting. When this
        URL is opened in a web browser, the GoToMeeting client will be downloaded
        and launched and the meeting will start. The end user is not required to login
        to a client.
      operationId: MeetingsStartByMeetingIdGet
      x-api-path-slug: meetingsmeetingidstart-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: meetingId
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Link
  /meetings/{meetingId}:
    get:
      summary: Meeting
      description: Returns the meeting details for the specified meeting.
      operationId: MeetingsByMeetingIdGet
      x-api-path-slug: meetingsmeetingid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: meetingId
      responses:
        200:
          description: OK
      tags:
      - Meeting
    put:
      summary: Meeting
      description: "Updates an existing meeting specified by meetingId.\r\n\r\n\t\t\t\t\t\t\t\t\t\t\r\n\t\tfield\t\t\tvalue\t\t\tdescription\t\t\r\n\t\t\"subject\"\t\t\t\"subject\"\t\t\tString
        - max 100 char.\t\t\r\n\t\t\"starttime\"\t\t\t\"2019-05-10T12:00:00Z\"\t\t\t{YYYY}-{MM}-{DD}T{HH}:{MM}:{SS}Z
        format, UTC only\t\t\r\n\t\t\"endtime\"\t\t\t\"2019-05-10T13:00:00Z\"\t\t\t{YYYY}-{MM}-{DD}T{HH}:{MM}:{SS}Z
        format, UTC only\t\t\r\n\t\t\"passwordRequired\"\t\t\tFALSE\t\t\tBoolean:
        true, false\t\t\r\n\t\t\"conferencecallinfo\"\t\t\t\"hybrid\"\t\t\tMust be
        one of: Hybrid, PTSN, Free, Private, VoIP.\t\t\r\n\t\t\"timezonekey\"\t\t\t\t\t\tAll
        times default to UTC\t\t\r\n\t\t\"meetingtype\"\t\t\t\"scheduled\"\t\t\tMust
        be one of: scheduled, recurring, immediate"
      operationId: MeetingsByMeetingIdPut
      x-api-path-slug: meetingsmeetingid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: meetingId
      responses:
        200:
          description: OK
      tags:
      - Meeting
    delete:
      summary: Meeting
      description: Deletes the meeting identified by the meetingId.
      operationId: MeetingsByMeetingIdDelete
      x-api-path-slug: meetingsmeetingid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: meetingId
      responses:
        200:
          description: OK
      tags:
      - Meeting
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