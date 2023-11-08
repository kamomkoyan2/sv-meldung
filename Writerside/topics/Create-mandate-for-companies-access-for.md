# Request Mandate for companies

<api-endpoint openapi-path="./../openapi.yaml" endpoint="/api/v1/mandate/request/apply" method="post">
    <response type="201">
        <sample>
            {
              "status": 201,
              "message": "Successfully created mandate"
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
<response type="409">
    <sample>
        {
          "status": 409,
          "error": "There is already an open mandate request for the specified company number. Please contact the company."
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
