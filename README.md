# bot9-frontend-assignment
Code the frontend for the following analytics UI.

Figma: https://www.figma.com/design/12eVe9Zeh948sZbynbQsRj/Analytics-Screen?node-id=0-1&t=28NkAsczNDghNf9B-1

Sample JSON (You do not need to connect to a backend): 
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

### Tech stack:
- NextJs (Pages router)
- TailwindCSS

### Todos:
1. Pixel perfect frontend.
2. On changing tabs lift the state up to a URL.
3. Graph is not required.
4. Make a custom `category bar` component for the breakdown sections.
5. Loading states when toggling between tabs.
6. Mobile responsive.

### Bonus:
1. Make a tooltip component for the `Support requests` tab with the following text: `Every conversation in inbox is marked as one support request. One visitor can have multiple support requests.`
2. Basic transitions using only tailwind css.
3. The sidebar and header as shown in the design.
