<h1>Prueba técnica de Kin+Carta resuelta con Next.js y Tailwindcss</h1>

Please build an app to showcase a small sample of some of the amazing work Kin + Carta Create has delivered over the years.

You are required to show the list of Kin + Carta Create case studies available here (https://raw.githubusercontent.com/theappbusiness/engineering-challenge/main/endpoints/v1/caseStudies.json). 
Please embed the URL below into your codebase. 
On launch, the app should always fetch the latest case studies from the given URL. 
If we add more case studies in the future, your app will display the up-to-date list. Do not read from hardcoded JSON. Do not embed images within the app, download them from the URLs provided within the JSON.

<h2>Requirements</h2>

The requirements are broken down into two user stories:

  -KCC-001: As a user, I want to see a list of case studies with an image and teaser.
  
  -KCC-002: As a user, I want to read the full article when I select a case study from the list.

<h3>KCC-001</h3>

When opening the app, the user should see the list of case studies available in the JSON at the given URL.

The user should see the list of case studies as per the array value for the "case_studies" key in the JSON.

For each case study in the list, the user should see:

  -a hero image, downloaded from the URL value provided for the "hero_image" key (do not embed images within the app);
   teaser text as per the "teaser" key in the JSON.

⚠️ Any case study JSON object with insufficient information should be ignored, e.g. if the "teaser" field is missing.

<h3>KCC-002</h3>

The user can navigate to read a full article by selecting a case study from the list.

For the full article, the user should see:

  -a hero image, downloaded from the URL value provided for the "hero_image" key (do not embed images within the app);
  
  -the title as per the "title" key;
   
  -body content broken into sections, as per the array value for the "sections" key;
  
For each section of body content, the user should see:

  -the section title (if provided in the JSON). This should be in a strong font weight to distinguish it from body text. It is read from the section's "title" key;
  
  -a list of body elements (either text or images). These are read from the "body_elements" key;
  
  -any images within the sections of body content should be downloaded from the URL provided for the image_url key.
  
The user should be able to easily return to the full list of case studies (delivered in KCC-001).
