The RFR application is slowing down every day. The processing time for calculations is increasing, and now it seems highly likely that it will exceed the configured and available time window for calculations. Consequently, publication will be delayed due to the search functionality issue between RFR and CFS when attempting to publish back to CFS.
We have two issues: firstly, the application is slowing down, and secondly, the RD library crashes randomly. This is problematic because when the session library crashes, we lose access to CFS and other services, rendering us unable to download or upload anything.
@Sathapanapatr, Ekachai from the CFS team has checked and confirmed that no errors were found from the RDP gateway.
After the investigation, we suspect there is an issue with the RD library, and the 502 Bad Gateway error appears to be from the CFS side. Therefore, the AAA team needs to figure out the issues. I have attached a screenshot of the 502 Bad Gateway request.
@Vilchynskyi, Yurii (External) from the STS team has confirmed that there was a network glitch at 11:21 GMT in the EU-WEST region.
@Havrylevych, Dmytro (External) from STS team has shared the logs and indicated them as “seems like the time we had increased 5xx is 11:18 and the time when you had errors in logs was 11:21, while we have zero errors at that time”, also attached a screenshot of the logs here.


