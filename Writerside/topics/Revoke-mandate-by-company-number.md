# Revoke Mandate by company number

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api/v1/mandate/revoke/{companyNumber}" method="post">
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
