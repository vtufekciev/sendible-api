To create a support ticket on behalf of the authenticated user, make a POST request.

#### URL: ####
http://sendible.com/api/v2/support_ticket.json

#### HTTP Methods: ####
POST

#### Parameters: ####
  * `application_id`: Your application id from http://sendible.com/developers.
  * `subject`: This is the ticket title/subject.
  * `message`: This is the ticket description.
  * `mode`: Optional. Use `test` if in development or `live` to store tickets in the live support system.

#### Authentication: ####
Basic authentication with username and password or remote API key belonging to the Sendible user.

#### Success Response: ####
```
{
    "ticket": {
        "url": "https://mysite.zendesk.com/api/v2/tickets/8.json",
        "id": 8,
        "external_id": null,
        "via": {
            "channel": "api",
            "source": {
                "from": {
                    
                },
                "to": {
                    
                },
                "rel": null
            }
        },
        "created_at": "2013-10-29T17:07:39Z",
        "updated_at": "2013-10-29T17:07:39Z",
        "type": null,
        "subject": "Hi",
        "description": "test",
        "priority": null,
        "status": "open",
        "recipient": null,
        "requester_id": 527109896,
        "submitter_id": 527109896,
        "assignee_id": 521231896,
        "organization_id": null,
        "group_id": 21395086,
        "collaborator_ids": [
            
        ],
        "forum_topic_id": null,
        "problem_id": null,
        "has_incidents": false,
        "due_at": null,
        "tags": [
            
        ],
        "custom_fields": [
            
        ],
        "satisfaction_rating": null,
        "sharing_agreement_ids": [
            
        ],
        "fields": [
            
        ]
    },
    "audit": {
        "id": 19529650186,
        "ticket_id": 8,
        "created_at": "2013-10-29T17:07:39Z",
        "author_id": 521231896,
        "via": {
            "channel": "api",
            "source": {
                "from": {
                    
                },
                "to": {
                    
                },
                "rel": null
            }
        },
        "metadata": {
            "system": {
                "ip_address": "174.129.96.109",
                "location": "Ashburn, VA, United States",
                "latitude": 39.0437,
                "longitude": -77.4875
            },
            "custom": {
                
            }
        },
        "events": [
            {
                "id": 19529650206,
                "type": "Comment",
                "author_id": 527109896,
                "body": "test",
                "html_body": "
test

",
                "public": true,
                "trusted": true,
                "attachments": [
                    
                ]
            },
            {
                "id": 19529650216,
                "type": "Create",
                "value": "Hi",
                "field_name": "subject"
            },
            {
                "id": 19529650226,
                "type": "Create",
                "value": "open",
                "field_name": "status"
            },
            {
                "id": 19529650236,
                "type": "Create",
                "value": null,
                "field_name": "priority"
            },
            {
                "id": 19529650246,
                "type": "Create",
                "value": null,
                "field_name": "type"
            },
            {
                "id": 19529650256,
                "type": "Create",
                "value": "521231896",
                "field_name": "assignee_id"
            },
            {
                "id": 19529650266,
                "type": "Create",
                "value": "21395086",
                "field_name": "group_id"
            },
            {
                "id": 19529650276,
                "type": "Create",
                "value": "527109896",
                "field_name": "requester_id"
            },
            {
                "id": 19529650286,
                "type": "Notification",
                "via": {
                    "channel": "rule",
                    "source": {
                        "to": {
                            
                        },
                        "from": {
                            "id": 40732486,
                            "title": "Notify requester of received request"
                        },
                        "rel": "trigger"
                    }
                },
                "subject": "Request received: {{ticket.title}}",
                "body": "Your request ({{ticket.id}}) has been received and is being reviewed by our support staff.\n\nTo add additional comments, reply to this email.\n
{{ticket.comments_formatted}}]",
                "recipients": [
                    527109896
                ]
            }
        ]
    }
}
```