# awesome-chatbot-models
List of existing models that can be picked up for chatbot training

## Dialog models

1. QBox Chatbot Model for general purpose intents about epidemic situation with the company and intents about company state (is it open, is deliver working).
    * Use this model to quickly rollout intents to inform users about current situation regarding epidemic. 
    * Use it to extend your current bot by just adding needed intents.

    **Links** [post](https://medium.com/qbox-nlp-performance-tooling/new-model-for-rapid-deployment-of-covid-19-trained-chatbots-8806fb94a8ff), [model](https://github.com/benoitalvarez/Covid-19-QBox-ChatbotModel)

    **NLU exports**: Dialogflow, Watson, LUIS, Rasa

    **Languages** English


## Knowledge Bases (Question-Answer)

1. Chit-chat QnA Maker dataset. Pre-populated set of the top chit-chat intents. 
    * Use this model to make a bot more conversational and engaging from the beginning. The model can be converted to other SaaS NLU format.

    * The model has 5 types of bot answers based on a different personality. Use this model to evaluate what alternative personalities exist. 

    **Links**: [docs](https://docs.microsoft.com/en-us/azure/cognitive-services/qnamaker/how-to/chit-chat-knowledge-base), [model](https://github.com/Microsoft/BotBuilder-PersonalityChat/tree/master/CSharp/Datasets). 

    **NLU exports**: Q&A Maker 
 
    **Languages**: Chinese, English, French, German, Italian, Japanese, Korean, Portuguese, Spanish.

1. Dialogflow small talk model has most of the required intents to start to build a bot from scratch. It contains not only small talk intents but a wider list of confirmation/declining/... phrases that can be reused for some multi-turn dialogs.
    * Use it when creating greenfield bot to enable wider topics from the beginning.
    * Add some intents to an existing bot to extend the number of topics bot can answer.
    * Use it to add a small talk to existing bot.

    **Links**: [docs](https://cloud.google.com/dialogflow/docs/agents-small-talk), [manual model export](https://github.com/spzm/dialogflow-smalltack-export)

    **NLU exports**: Dialogflow

    **Languages**: English