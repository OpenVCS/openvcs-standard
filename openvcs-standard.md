<h3>OpenVCS 0.2</h3>
*Groups may provide explicit opt-in to be included in the data set, so in my own exports I also include a field to check the opt-in (called 'directory consent' yes/no), but this is stripped out of the open data once it has been checked as it has then served its purpose. Postcodes are used to provide geocode (map point) data. Where a small group's address is a residential address, an individual could be identified as connected to that group presenting a potential breach of data protection. If groups wish, they can provide a slightly altered postcode. In the majority of cases this is not an issue and may not be an issue at all - depending on your local situation.

When making your data available in the OpenVCS format (as a CSV or Excel file for example) I suggest posting it to your website domain at /open. For example yourdomain.com/open. I also suggest a naming convention for the file as follows:

openvcs-v02-ocva.csv where 'openvcs' identifies the data format, 'v02' identifies the version of openvcs in use (version 0.2 in this case) and 'ocva' identifies the name of your organisation (for me it's OCVA, Oxfordshire Community & Voluntary Action). I'd suggest not putting the date in the file name because that would change the file name each time. But you could put the date of the data export on its related web page, or even in the text of the link to the file. 

Our format is derived from CiviCRM.  and uses the following fields. Replace {AREA} with county or city name (for example, Oxfordshire) and {REGION} with UK region (for example South East Region):
<table border="1" summary="This table describes the OpenVCS data format" cellspacing="2" cellpadding="1"><caption>OpenVCS</caption>
<tbody>
<tr>
<th>Field</th>
<th>Description</th>
<th>Required, Recommended (mapped to a national schema), Optional?</th>
<th>Root source for this</th>
</tr>
<tr>
<td>Display Name</td>
<td>Legal or registered name</td>
<td>Required</td>
<td></td>
</tr>
<tr>
<td>State</td>
<td>County</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Website</td>
<td>Main URI</td>
<td>Recommended</td>
<td></td>
</tr>
<tr>
<td>Type of Organisation</td>
<td><strong>Choose from:</strong> Unincorporated association, club or group with a constitution; Community association, club, group without a constitution; Network or Partnership; Registered charity or trust; Charitable Incorporated Organisation (CIO);
Community Interest Company (limited by guarantee or shares); Co-operative; Company limited by guarantee (inc LLP); Registered social landlord; Company limited by shares; Industrial and Provident Society cooperative; Industrial and Provident Society community benefit; Other</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Sector</td>
<td><strong>Choose from: </strong>Voluntary &amp; Community; Private; Statutory; Academic</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Charity Number</td>
<td>For registered charities</td>
<td>Recommended</td>
<td>Charity Commission UK</td>
</tr>
<tr>
<td>Company Number</td>
<td>For registered companies</td>
<td>Recommended</td>
<td>Companies House UK</td>
</tr>
<tr>
<td>Number of Employees</td>
<td>Numeric</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Number of other volunteers</td>
<td>Numeric</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Funding Sources</td>
<td><strong>Choose from: </strong>Corporate donations or sponsorship; Funding from EC sources (e.g European social fund); Fundraising from the general public (inc legacies); Grants from trusts or the National lottery; Grants or contracts from an NHS body; Grants or contracts from an {AREA} local authority; Grants or contracts from {AREA} County Council; Grants or contracts from {AREA} City Council; Grants or contracts from {AREA} District Council; Investment income; local authority/regional grants outside {AREA}; Membership fees; No income; Rental income; Trade (Sale of goods or charges for services)</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Last years' income</td>
<td><strong>Choose from: </strong>Less than £5,000 (A); £5,000 - £24,999 (B); £25,000 - £49,999 (B); £50,000 - £99,000 (B); £100,000 - £249,000 (B2); £250,000 - £499,000 (C); £500,000 - £999,000 (C); £1million or more (C)</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>What you do, and what you need</td>
<td>Text description from which keywords can be extracted. Suggested help text: 'Explain in simple terms your service, any current needs you have (volunteers, funds, building, skills)'</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Type of Service</td>
<td><strong>Choose from: </strong>Advice and information; Animal Welfare; Campaigning; Community development &amp; community planning; Economic development (including regeneration and employment); Emotional support (e.g. befriending, counselling bereavement support etc); Religious teaching; Financial services (inc Credit Union); Health; International development; Play/ Youth work; Social care and welfare; Transport; Advocacy; Arts, Media and culture; Community centre / village hall; Community safety / criminal justice; Education &amp; training; Environment and conservation; Worship, Prayer and Meditation; Grant making trust; Housing &amp; hostels; Mediation and brokerage; Research and development; Sport &amp; recreation</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Client Groups</td>
<td><strong>Choose from: </strong>Children (age 0 - 15); Young People (age 16 - 25); NEET; Older People (age 50 +); Carers; Families and Parents; Women; Men; Lesbian, Gay, Bi-sexual and Transgender people; Gypsies and travellers; Homeless people; Offenders, ex- offenders, those at risk of offending; Refugees and asylum seekers; Service and ex-service people; Unemployed people; Victims of crime, violence or abuse; Black and ethnic minority people; People of a particular religion, faith or culture; People with a learning disability; People with a physical disability; People with a sensory disability; Drug, alcohol and substance users; People with a medical condition; People with mental health issues; Voluntary organisations and community groups; All members of the community; Animals; The environment</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Geographic Areas Service is Provided</td>
<td><strong>Choose from: </strong>{AREA} City, {AREA} District(s), {AREA} and adjacent counties, {REGION}, UK, Outside UK</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Wards covered in {AREA}</td>
<td>A list of ward codes in the 2011 census format. (Example Cherwell E05006517 Adderbury). Includes option for 'ALL'.</td>
<td>Optional</td>
<td>UK Census</td>
</tr>
<tr>
<td>Geo Code 1</td>
<td>Latitude or Longitude numeric. Derived from postcode (not shared).*</td>
<td>Required</td>
<td></td>
<tr>
<td>Geo Code 2</td>
<td>Latitude or Longitude numeric. Derived from postcode (not shared).*</td>
<td>Required</td>
<td></td>
</tr>
<tr>
<td>Project of-display_name</td>
<td>Text field for organisations with a parent body, giving parent body's name</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Postal Code</td>
<td>A valid UK Postcode</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Date Disbanded</td>
<td>Date range in the format DD/MM/YYYY</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>IMPACT Categories</td>
<td>These come from UKCF and you can <strong>Choose from:</strong> Improve peoples education employability and enterprise; Maximise peoples ability to strengthen community cohesion and build social capacity; Provide people with opportunity to address greater social justice and reduce exclusion and disadvantage; Advance peoples physical and mental health wellbeing and safety; Connect people with the arts culture and heritage; Transform peoples access to and engagement with their environment and public services</td>
<td>Recommended</td>
<td>UKCF members</td>
</tr>
<tr>
<td>Federated with/ Affiliated to/ Ex-affiliated to</td>
<td>Text field for organisations to explain their professional memberships</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>This contact is for:</td>
<td><strong>Choose from:</strong> A service; An organisation; A facility</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>What are the requirements of people who want to use this service?</td>
<td>Text field.</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Hours of Operation (eg, "9:00 - 15:00 Monday to Friday")</td>
<td>Text field. Preferred format like: "09:00 - 17:00 Monday to Friday"</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Has worked with local VCS</td>
<td><strong>Choose from:</strong> Yes; No</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Date of this update</td>
<td>Date range in the format DD/MM/YYYY (a note of when this organisation's details were last updated)</td>
<td>Optional</td>
<td></td>
</tr>
<tr>
<td>Source of Contact Data</td>
<td>Text field. Source of the data in the record. For example 'google' or 'local foundation'</td>
<td>Optional</td>
<td></td>
</tr>
</tbody>
</table>

