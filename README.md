# Alexa Skill - Chat with Gemini
### Alexa Skill Template to Integrate Google Gemini on Alexa Devices

**Credit to [Scintilla Hub](https://www.youtube.com/@scintillahub)**

## Requirements
* With a Google account, generate an authentication key at [Google AI Developer](https://ai.google.dev/). Copy and save the key, it will only be visible at the time of creation.
* Create an account at [Amazon](https://www.amazon.com/ap/signin?openid.pape.preferred_auth_policies=Singlefactor&clientContext=132-2293245-7926858&openid.pape.max_auth_age=7200000&openid.return_to=https%3A%2F%2Fdeveloper.amazon.com%2Falexa%2Fconsole%2Fask&openid.identity=http%3A%2F%2Fspecs.openid.net%2Fauth%2F2.0%2Fidentifier_select&openid.assoc_handle=amzn_dante_us&openid.mode=checkid_setup&marketPlaceId=ATVPDKIKX0DER&openid.claimed_id=http%3A%2F%2Fspecs.openid.net%2Fauth%2F2.0%2Fidentifier_select&openid.ns=http%3A%2F%2Fspecs.openid.net%2Fauth%2F2.0&) and log into _Alexa Developer Console_.
## Creating the Alexa Skill
Create an Alexa-hosted Skill (Python) on Alexa: (_Create Skill_)

1. Name your Skill: Choose a name of your choice, e.g., Chat with Gemini
2. Choose a primary locale, e.g., Portuguese (BR)
3. Click _Next_. In Experience Type, select: Other > Custom > _Alexa-hosted (Python)_
4. _Hosting region_: You can leave the default _US East (N. Virginia)_
5. In _Templates_: Click _Import Skill_
6. Enter the repository address: https://github.com/WandLZhang/alexa-skill-gemini.git and confirm.

## Configuring the Skill
When you finish importing _Invocations_ > _Skill Invocation Name_:
1. Edit _Skill Invocation Name_. This will be the invoking command for your skill. Pay attention to word requirements and restrictions.
2. Click _Save_
3. Build the Skill by clicking _Build Skill_. When finished, go to the tab **Code**
4. Create a file inside the Lambda folder called _.env_ and add the line, adding the generated API key:
   ```shell
   GOOGLE_API_KEY=SuaApiKeyGoogleAI
   ```
5. Click _Save_ and then click _Deploy_
   
## Test the Skill
When _deploy_ finishes, go to the tab **Test**:
1. In _Skill testing is enabled in_, turn it from _Off_ to _Development_
2. To use voice commands, accept the website's request to use the microphone, and to speak, click and hold the mic icon, and release to send
3. Use the configured activation command to start the Skill, and you're ready to interact with Gemini via Alexa!

The Skill will now be available on all Alexa devices linked to your account.
