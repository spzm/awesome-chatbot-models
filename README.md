# awesome-chatbot-models
List of existing models to boost the start of the chatbot project. How do I start with it? Review the intents in the models, pick up the ones that fit the domain, clean up utterances and entities that are not fit and add them to the bot. It helps to build the chatbot base much quicker. Also, I don't forget to learn from these examples - the design of intents and entities there, the rules developers follow. Important to note, even existing production-intent data won't guarantee a success factor - it's just the beginning - it will require additional training when real users start chatting.

## Dialog models

1. Carbon Bot. This is a real bot example that can be found in [facebook messenger](https://m.me/CarbonBot.from.Rasa). Dialogs, NLU model, and fulfillment actions to calculate the emissions from air travel, suggest UN-certified projects you can donate to. The model contains full-featured intents: small talks, checking emotions, vulgar questions, faq, domain intents. Worth to look intents - flight route - utterances from it can be easily reused for any other flight query. 

    **NLU exports**: Rasa

    **Links** [model](https://github.com/RasaHQ/carbon-bot/tree/master/data)
    
    **Languages** English

1. QBox Chatbot Model for general-purpose intents about the epidemic situation with the company and intents about company state (is it open, is deliver working).
    * Use this model to quickly rollout intents to inform users about the current situation regarding the epidemic. 
    * Use it to extend your current bot by just adding needed intents.

    **Links** [post](https://medium.com/qbox-nlp-performance-tooling/new-model-for-rapid-deployment-of-covid-19-trained-chatbots-8806fb94a8ff), [model](https://github.com/benoitalvarez/Covid-19-QBox-ChatbotModel)

    **NLU exports**: Dialogflow, Watson, LUIS, Rasa

    **Languages** English

1. Rasa Helpdesk Assistant demo. Example of dialogs, NLU model, and fulfillment actions to open/track/close the ticket in the helpdesk system. This is just an example but good to use as a starting point for the domain.

    **NLU exports**: Rasa

    **Links** [model](https://github.com/RasaHQ/helpdesk-assistant/tree/master/data)
    
    **Languages** English

1. Rasa Financial Assistant demo. Example of dialogs, NLU model, and fulfillment actions to check balance, search transactions, transfer money, ask about transfer price, check earnings. This is just an example but good to use as a starting point for the domain.

    **NLU exports**: Rasa

    **Links** [model](https://github.com/RasaHQ/financial-demo/blob/master/data/nlu/nlu.md)
    
    **Languages** English





## Intents & entities models

1. RASA Crowd-sourced NLU training data

    RASA community launch a collective crowdsourcing initiative to provide basic training data for developing chatbots. Intents stored without entities markup but some of the intents represent a list of possible entity values. The Mixed-smalltalk+transport model has examples of multi-intent utterances. Currently, models have a small number of intents (up to 10) but it is in the active crowd-sourcing phase.

    Current domains: education, banking, buy a car, fixing_internet, mixed-smalltalk+transport, mood, restaurant-table-reservation, retail, small talk, weather 

    **Links** [model](https://github.com/RasaHQ/NLU-training-data)

    **NLU exports**: Rasa

    **Languages** English


## Knowledge Bases (Question-Answer)

1. Chit-chat QnA Maker dataset. Pre-populated set of the top chit-chat intents. 
    * Use this model to make a bot more conversational and engaging from the beginning. The model can be converted to other SaaS NLU format.

    * The model has 5 types of bot answers based on a different personality. Use this model to evaluate what alternative personalities exist. 

    **Links**: [docs](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/how-to/chit-chat-knowledge-base), [model](https://github.com/Microsoft/BotBuilder-PersonalityChat/tree/master/CSharp/Datasets). 

    **NLU exports**: Q&A Maker 
 
    **Languages**: Chinese, English, French, German, Italian, Japanese, Korean, Portuguese, Spanish.

1. Dialogflow small talk model has most of the required intents to start to build a bot from scratch. It contains not only small talk intents but a wider list of confirmation/declining/... phrases that can be reused for some multi-turn dialogs.
    * Use it when creating a greenfield bot to enable wider topics from the beginning.
    * Add some intents to an existing bot to extend the number of topics the bot can answer.
    * Use it to add a small talk to the existing bot.

    **Links**: [docs](https://cloud.google.com/dialogflow/docs/agents-small-talk), [manual model export](https://github.com/spzm/dialogflow-smalltack-export)

    **NLU exports**: Dialogflow

    **Languages**: English