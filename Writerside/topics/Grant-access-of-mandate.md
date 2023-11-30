# Grant Access Of Mandate

<!--You can use any other Markdown or XMl elements around the API endpoint reference,
for example, put API endpoints in chapters or tabs. -->

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/mandate/confirm/{companyNumber}" method="post">
    <response type="200">
        <sample>
            {
              "status": 200,
              "message": "Successfully granted mandate"
            }
        </sample>
    </response>
<response type="404">
    <sample>
        {
          "status": 404,
          "error": "The company number you entered does not exist"
        }
    </sample>
</response>
<response type="500">
    <sample>
        {
          "status": 500,
          "error": "Internal server error"
        }
    </sample>
</response>
</api-endpoint>
