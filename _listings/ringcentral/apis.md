---
name: RingCentral
x-slug: ringcentral
description: 'RingCentral, Inc. (NYSE: RNG) is a global provider of cloud enterprise
  unified communications and collaboration solutions. More flexible and cost-effective
  than legacy on-premise systems, RingCentral empowers today&rsquo;s mobile and distributed
  workforces to be connected anywhere and on any device through voice, video, team
  messaging, collaboration, SMS, conferencing, online meetings, contact center, and
  fax. RingCentral provides an open platform that integrates with today&rsquo;s leading
  business apps while giving customers the flexibility to customize their own workflows.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
x-kinRank: "7"
x-alexaRank: "7180"
tags: Meetings
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/apis.md
specificationVersion: "0.14"
apis:
- name: RingCentral Connect Platform API Explorer - Get Scheduled Meetings [Beta]
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeeting-get
  description: |-
    Returns a list of meetings for a particular extension. The list of meetings does not include meetings of &#39;Instant&#39; type.
    App Permission
    Meetings
    User Permission
    Meetings
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeeting-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeeting-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Meetings [Beta]
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeeting-post
  description: "Creates a new meeting.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [schedule] value is invalid\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeeting-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Meeting Info [Beta]
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get
  description: "Returns a particular meetings details by ID.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put
  description: "Modifies a particular meeting.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [password] value is invalid\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete
  description: |-
    Deletes a scheduled meeting.
    App Permission
    Meetings
    User Permission
    Meetings
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - End Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post
  description: "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Meeting Service Info
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get
  description: "Returns information on dial-in numbers for meetings, support and international
    dial-in numbers URIs and meeting account information.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call this
    API endpoint, application needs to have [Meetings] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [Meetings] permission for
    requested resource."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Meeting Info [Beta]
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get
  description: "Returns a particular meetings details by ID.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put
  description: "Modifies a particular meeting.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [password] value is invalid\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete
  description: |-
    Deletes a scheduled meeting.
    App Permission
    Meetings
    User Permission
    Meetings
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - End Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post
  description: "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Meeting Service Info
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get
  description: "Returns information on dial-in numbers for meetings, support and international
    dial-in numbers URIs and meeting account information.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call this
    API endpoint, application needs to have [Meetings] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [Meetings] permission for
    requested resource."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Meeting Service Info
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get
  description: "Returns information on dial-in numbers for meetings, support and international
    dial-in numbers URIs and meeting account information.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call this
    API endpoint, application needs to have [Meetings] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [Meetings] permission for
    requested resource."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get-openapi.md
- name: RingCentral Connect Platform API Explorer - End Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post
  description: "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-openapi.md
- name: RingCentral Connect Platform API Explorer - End Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post
  description: "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-openapi.md
- name: RingCentral Connect Platform API Explorer - End Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post
  description: "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete
  description: |-
    Deletes a scheduled meeting.
    App Permission
    Meetings
    User Permission
    Meetings
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete
  description: |-
    Deletes a scheduled meeting.
    App Permission
    Meetings
    User Permission
    Meetings
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete
  description: |-
    Deletes a scheduled meeting.
    App Permission
    Meetings
    User Permission
    Meetings
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put
  description: "Modifies a particular meeting.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [password] value is invalid\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put
  description: "Modifies a particular meeting.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [password] value is invalid\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Meeting Info [Beta]
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get
  description: "Returns a particular meetings details by ID.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Meeting Info [Beta]
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get
  description: "Returns a particular meetings details by ID.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/meetings/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/ringcentral-developers
- type: x-blog-rss
  url: https://medium.com/feed/ringcentral-developers
- type: x-github
  url: https://github.com/ringcentral
- type: x-openapi
  url: https://netstorage.ringcentral.com/dpw/api-explorer/swagger-ring_basic.yml?v=20180816
- type: x-website
  url: http://www.ringcentral.com
- type: x-api-gallery
  url: http://reverb.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ringcentral.stack.network
- type: x-code
  url: https://developer.ringcentral.com/library/sdks.html
- type: x-crunchbase
  url: https://crunchbase.com/organization/ringcentral
- type: x-developer
  url: https://developer.ringcentral.com/
- type: x-documentation
  url: https://developer.ringcentral.com/api-explorer/latest/index.html?_ga=2.259782990.551967760.1534465156-1236351744.1533920460
- type: x-support
  url: https://developer.ringcentral.com/support.html
- type: x-twitter
  url: https://twitter.com/RingCentral
- type: x-website
  url: https://developer.ringcentral.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---