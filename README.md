# bot9-frontend-assignment
Code the frontend for the following analytics UI.

Figma: https://www.figma.com/design/12eVe9Zeh948sZbynbQsRj/Analytics-Screen?node-id=0-1&t=28NkAsczNDghNf9B-1

Sample JSON (You do not need to connect to a backend):

`Visitor`'s Tab -

```
{
    "common": {
        "visitorCount": {
            "value": 369,
            "percentChange": 100,
            "info": ""
        },
        "supportRequestCount": {
            "value": 629,
            "percentChange": 100,
            "info": ""
        },
        "medianResponseTime": {
            "value": 2.786,
            "percentChange": 100,
            "info": ""
        },
        "customerScore": {
            "value": 0,
            "percentChange": 0,
            "info": ""
        }
    },
    "detailed": {
        "interactionBreakdown": [
            {
                "name": "Generated new support request",
                "percent": "150.12",
                "count": 629
            },
            {
                "name": "Replied to message or bot",
                "percent": "0.24",
                "count": 1
            },
            {
                "name": "No interaction",
                "percent": "0.24",
                "count": 1
            }
        ],
        "visitorTypeBreakdown": [
            {
                "name": "Visitor",
                "percent": "85.42"
            },
            {
                "name": "Lead",
                "percent": "11.57"
            },
            {
                "name": "Customer",
                "percent": "3.01"
            }
        ],
        "locationBreakdown": [
            {
                "name": "Bengaluru, KA, IN",
                "percent": "77.09"
            },
            {
                "name": "Eluru, AP, IN",
                "percent": "10.26"
            },
            {
                "name": "IN",
                "percent": "3.82"
            },
            {
                "name": "Vijayawada, AP, IN",
                "percent": "2.63"
            },
            {
                "name": "Unknown",
                "percent": "1.91"
            }
        ]
    }
}
```

`Support request`'s tab - 

```
{
    "common": {
        "visitorCount": {
            "value": 369,
            "percentChange": 100,
            "info": ""
        },
        "supportRequestCount": {
            "value": 629,
            "percentChange": 100,
            "info": ""
        },
        "medianResponseTime": {
            "value": 2.786,
            "percentChange": 100,
            "info": ""
        },
        "customerScore": {
            "value": 0,
            "percentChange": 0,
            "info": ""
        }
    },
    "detailed": {
        "requestTypeBreakdown": [
            {
                "name": "Others",
                "percent": "83.23"
            },
            {
                "name": "General Inquiry",
                "percent": "5.22"
            },
            {
                "name": "Account Signup",
                "percent": "5.22"
            },
            {
                "name": "Technical Issues",
                "percent": "3.48"
            },
            {
                "name": "Account Login",
                "percent": "2.85"
            }
        ],
        "requestPriorityBreakdown": [
            {
                "name": "Moderate",
                "percent": "41.11"
            },
            {
                "name": "Low",
                "percent": "32.22"
            },
            {
                "name": "Urgent",
                "percent": "26.67"
            }
        ],
        "resolutionStatusBreakdown": [
            {
                "name": "Bot",
                "percent": "81.80"
            },
            {
                "name": "Closed",
                "percent": "9.81"
            },
            {
                "name": "Agent",
                "percent": "8.39"
            }
        ]
    }
}
```

### Tech stack:
- NextJs (Pages router)
- TailwindCSS

### Todos:
1. Pixel perfect frontend.
2. On changing tabs lift the state up to a URL. The URL state should persist on reload.
3. Graph is not required.
4. Make a custom `category bar` component for the breakdown sections.
5. Loading state when toggling between tabs.
6. Mobile responsive.
7. Make a tooltip component for the `Support requests` tab with the following text: `Every conversation in inbox is marked as one support request. One visitor can have multiple support requests.`
8. Proper project structure.

### Bonus:
1. Basic transitions using only tailwind css.
2. The sidebar and header as shown in the design.
