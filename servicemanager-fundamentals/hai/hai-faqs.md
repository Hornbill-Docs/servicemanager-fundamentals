---
layout: article-toc
---

# HAi FAQs

## Overview

These FAQs, grouped by topic, are designed to support queries regarding the HAi model and how HAi operates. 

HAi uses third-party AI Providers, including OpenAI and Azure OpenAI, for certain AI capabilities.

Hornbill is responsible for the HAi application, including the data and context supplied to the AI service, application-level access controls, orchestration, guardrails, human approval mechanisms and auditability.

The third-party AI Provider is responsible for the underlying AI model, including its model training, model-level safety controls and model-level fairness and bias evaluation. 

The respective responsibilities are governed by the applicable contractual and data-processing arrangements.

## Hornbill AI Usage Policy

The usage of Hornbill AI is governed by the [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf), as well as section 3.4 of the [Hornbill Subscription Agreement](https://www.hornbill.com/subscription-agreements) however HAI is subject to additional terms based on which [HAi Provider](/servicemanager-config/administration/hai-providers) is being used, Azure AI Services or OpenAI.

## Performance and Scalability

### What are the expected response times for the AI model?

Hornbill Ai (HAi) delivers rapid response times averaging about 0.5 seconds to start generating output (Time to First Character or TTFC), with full responses completing in roughly 3.4 seconds depending on the underlying model configuration.

### How does the system handle peak loads and high traffic?

HAi handles high traffic and peak loads by relying on the scalable cloud infrastructure of world-class external model providers like OpenAI and Azure OpenAI Service, processing requests asynchronously via enterprise-grade API integrations rather than hosting resource-heavy models locally.

### How does HAi scale to accommodate increasing amounts of data or users?

HAi is built on a cloud-native SaaS architecture designed to scale horizontally and accommodate growing enterprise user bases and data demands.

### How is system availability maintained?

HAi and the broader Hornbill platform are designed for continuous delivery with zero scheduled downtime for regular updates. Essential infrastructure patches or minor maintenance may occasionally require up to two minutes of downtime, typically scheduled outside working hours (at 05:00 UTC for platforms and 05:30 UTC for applications, Monday through Friday).

### How can AI usage and performance be monitored?

HAi includes a dashboard providing real-time metrics to monitor organizational AI usage, supporting operational reporting on usage and performance.

For generative AI, traditional model-quality measures such as accuracy, precision and recall are not typically reported in the same way as they are for fixed classification models. Quality assurance measures can instead be defined as part of organizational governance and acceptance testing.

HAi also incorporates human-in-the-loop controls, with users expected to review and validate HAi’s proposals before they are actioned. This supports appropriate human oversight of the accuracy and suitability of AI-generated outputs.

## Usability

### How easy is HAi to use?

HAi is designed to be user-friendly and intuitive. Generative AI is embedded directly into the Hornbill platform at specific points of need, with single-click activation and no special technical skills required.

HAi Insights windows and Assistants (chatbots) are also available at specific points of need and can be expanded or collapsed with a single click.

HAi is managed by Hornbill Administrators with the appropriate roles and permissions. HAi Control provides a central, contained area for configuring and monitoring all HAi tools.

### What guidance and training is available for HAi?

Hornbill provides comprehensive documentation and online training to support the use of HAi, including technical reference information, guidance and best practices.

Hornbill Documentation provides [technical reference information](/servicemanager-config/administration/hai) and [guidance](/servicemanager-user-guide/hai/overview), while the [Hornbill Academy](https://academy.hornbill.com) provides structured online learning.

Hornbill Administrators are required to complete a relevant Learning Path before HAi is activated, ensuring they understand the prerequisites, controls, the context of AI for Service Management, and their responsibilities and associated risks.

In Q3 2026, Hornbill will release a comprehensive Learning Path for Service Desk Agents to support the responsible use of HAi tools.

All HAi documentation and training materials are available to customers at no additional cost.

### How does HAi provide transparency and auditability of AI interactions?

The internal reasoning processes of AI models are not transparent in the sense that users cannot see the model's private chain of thought or every internal computational step used to generate a response.

However, HAi provides auditability of AI interactions. Subject to the capabilities of the relevant HAi feature, Hornbill maintains records that may include the user or AI Agent initiating a request, the date and time, the AI capability or model used, relevant inputs and outputs, and actions initiated or performed. This provides visibility into the information supplied to the model and the resulting response, without exposing the model's private internal reasoning.

These records also support governance, security monitoring and investigation of reported issues or inappropriate use.

## Model development

### Is customer data used to train AI models?

No customer data is used to train AI models.

### How does HAi incorporate human oversight?

Human oversight is required for HAi-generated recommendations and content before they are implemented or used where the HAi capability requires an approval or user action.

HAi can generate suggestions, proposed actions and content, but the user remains responsible for reviewing and approving the resulting action. For example, HAi may generate a customer email, suggest a resolution to a service request, or create a draft knowledge article based on a resolved request. The user can review, amend, approve or reject the recommendation before it is used or applied.

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) requires customers to implement sufficient human oversight for their use of HAi and specifically prohibits certain consequential decisions being made solely on the basis of HAi output.

### How can users review and override HAi recommendations or proposed actions?

HAi does not independently implement consequential decisions or actions without appropriate human oversight. Recommendations and proposed actions remain subject to review and approval by an appropriately authorized user.

For example, HAi may recommend sending an email to a customer and generate a draft email. HAi presents this as a suggested next step; it does not send the email automatically. The user is responsible for reviewing, editing, approving or rejecting the proposed action.

Similarly, where HAi generates written content, such as a draft email or knowledge article, the user can review and amend the content before it is used.

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) also expressly requires appropriate human oversight and prohibits using HAi as the sole basis for decisions that may materially affect an individual's legal rights, employment, financial position, health, safety or access to essential services without appropriate human review and oversight.

### What AI technologies and methodologies does HAi use?

HAi uses large language models (LLMs) and other machine-learning technologies provided by Hornbill and third-party AI Providers, including OpenAI and Azure OpenAI. The underlying models use neural-network and transformer-based architectures and generate outputs based on the input, contextual information and instructions provided to them.

HAi itself provides the application, orchestration, context and controls around these underlying models. The specific AI model or provider used may vary depending on the HAi capability.

### What data does HAi use to perform its functions?

The data provided to HAi is contextual and limited to the information required for the particular HAi capability to perform its function.

Depending on the capability, this may include:

- User-provided input, such as text entered into a dialog or prompt. For example, Text Assist generates a response based on the text submitted by the user.

- Contextual data retrieved by HAi, such as information associated with the record or activity on which the user is working. For example, the Suggest Resolution capability can use information from the service request timeline to generate a proposed resolution, without requiring the user to provide a separate prompt.

For capabilities that retrieve contextual data, HAi determines the relevant information based on the context of the user's request and their existing data entitlements. Only data that the user is authorized to access is made available to the model.

The specific data provided therefore varies by HAi capability and is limited to what is relevant to generating the requested response, recommendation or proposed action.

### How is data selected and prepared before it is provided to the AI model?

HAi does not expose the detailed data pre-processing, filtering or model preparation methodologies used by the underlying AI models, as these form part of the proprietary technology of Hornbill and its AI Providers.

At the HAi application level, data supplied to the model is selected according to the context of the relevant HAi capability and the user's existing data entitlements. HAi provides the model with the information required to perform the requested function rather than providing unrestricted access to the Customer's data.

The underlying AI model provider is responsible for its own model training and data-preparation processes. Further information on OpenAI's approach to data processing and privacy is available in its published documentation.

## Model Bias & Transparency

### How does HAi support transparency and auditability?

Transparency is supported through the following layers, although AI models cannot provide a complete, inspectable account of every internal computation that leads to an answer:

- Trace logging. HAi provides a trace log for AI operations. Depending on the HAi capability, this can include the data sent to and received from the AI model, associated API calls and other information about the execution of the AI operation. This provides visibility into the inputs, outputs and processing activity associated with an AI response, supporting investigation and governance.

- Human oversight. HAi recommendations and proposed actions can be reviewed by the user before they are implemented. This provides a human decision point where the user can assess, amend, approve or reject the AI-generated recommendation or content.

- AI provider policies and safety controls. The underlying AI models are provided by third-party AI Providers, whose policies and safety controls govern aspects of model behavior. These controls vary between AI Providers. For example, OpenAI publishes its Model Spec, which describes the intended behavior and principles governing its models.

It is important to distinguish transparency and auditability from full technical explainability. Neural networks are not inherently transparent, rule-based systems, and it is not generally possible to provide a simple, human-readable explanation of every internal computation that contributes to an individual response.

### How does HAi address fairness in AI-generated outputs?

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) acknowledges that AI and machine-learning technologies have known and unknown risks and limitations, including potential lack of fairness. It does not specify a particular methodology for ensuring fairness in the underlying AI models.

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) requires sufficient human oversight for the use of HAI and prohibits HAI from being used as the sole basis for certain decisions that may materially affect an individual's legal rights, employment, financial position, health, safety or access to essential services without appropriate human review and oversight.

For related information published by OpenAI, see:

- [OpenAI Model Spec](https://model-spec.openai.com/2026-08-18.html) documents intended model behavior, including fairness, objectivity, uncertainty and safety.

- [OpenAI: Evaluating fairness in ChatGPT](https://openai.com/index/evaluating-fairness-in-chatgpt/?utm_source=chatgpt.com) OpenAI describes an actual fairness evaluation looking at differences in responses associated with gender and race. 

### How does HAi address potential bias and discrimination?

The underlying AI models are provided by third-party AI Providers, who are responsible for model-level evaluation and mitigation of bias and harmful or discriminatory behavior. OpenAI, for example, publishes information about its approach to fairness and bias evaluation as part of its model safety and evaluation processes. See OpenAI: Evaluating fairness in ChatGPT.

Hornbill does not independently represent that the underlying model has been specifically validated against every protected characteristic listed in this questionnaire. The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) recognizes that AI technologies have known and unknown limitations, including potential bias and lack of fairness, and requires appropriate human oversight.

Customers should therefore apply appropriate organizational policies and human review when using HAi in circumstances where bias or discrimination could have material consequences.

### What safeguards are available to help identify and mitigate harmful or inappropriate AI outputs?

HAi provides several mechanisms for identifying and mitigating potentially harmful or inappropriate AI outputs.

The 2026 release of HAi provides Hornbill Administrators with the ability to define and manage guardrails, to help prevent or limit potentially harmful or inappropriate AI outputs. Hornbill provides out-of-the-box guardrails covering basic safeguarding requirements, and customers can define additional guardrails according to their organizational, compliance and HR requirements.

HAi also provides auditability of AI interactions to support investigation of reported issues. Under the [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf), customers can report inaccurate, unsafe, harmful, biased, unfair or inappropriate outputs to Hornbill for investigation and product improvement.

Customers should work with their relevant compliance, HR and governance teams to establish appropriate controls and review them as required.

### How can users report potential inconsistencies, bias or other concerns about HAi outputs?

Users can report suspected inconsistencies, inappropriate outputs or bias through the standard support and feedback mechanisms provided by Hornbill.

Where an issue relates to the underlying OpenAI model rather than HAi's implementation, Hornbill can investigate and, where appropriate, raise the issue with OpenAI through the channels available to API customers.

OpenAI also operates feedback and reporting mechanisms for model behavior and uses real-world feedback as part of its ongoing safety work

## Security

### What security measures and controls are in place for HAi?

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) requires Hornbill to maintain appropriate technical and organizational measures to support the monitoring and investigation of HAI activities. Hornbill may also implement security controls and may suspend or restrict access to HAI where reasonably necessary to protect the security, integrity or availability of the service, investigate or prevent suspected misuse or unlawful activity, comply with applicable law, or undertake maintenance or remediation activities.

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) does not provide a detailed description of Hornbill's underlying security architecture or individual security controls.

### What measures and controls help protect HAi against unauthorized access or data breaches?

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) does not provide a detailed description of Hornbill's technical measures for preventing unauthorized access or responding to data breaches.

It does state that Hornbill may implement security controls and may suspend or restrict HAI access where reasonably necessary to protect the security, integrity or availability of the service or to investigate or prevent suspected misuse or unlawful activity.

### How does HAi support audit logging, monitoring and diagnostics?

Subject to the capabilities of the relevant HAI feature, Hornbill maintains records of AI activity that may include the identity of the User or AI Agent, date and time, AI capability or model used, prompts or instructions where retained, outputs where retained, actions initiated or performed by AI Agents and other relevant metadata.

Where HAi recommends or initiates actions, Hornbill will use reasonable endeavors to maintain sufficient traceability to identify the originating prompt, instruction or triggering event, the AI capability responsible, whether human approval was required and the outcome.

These records support operational investigation, security monitoring and regulatory compliance. Audit records are retained in accordance with applicable law and Hornbill's retention policies.

### How does HAi support data integrity and consistency?

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) requires Hornbill to maintain appropriate technical and organizational measures in relation to HAI and permits Hornbill to implement controls or restrict access where reasonably necessary to protect the security, integrity or availability of the service.

However, the [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) does not specify the technical mechanisms used to ensure data integrity or consistency, such as validation, checksums, transactional controls or reconciliation processes. Those details are therefore outside the scope of the [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf).

## Compliance

### What regulations, standards and certifications apply to HAi?

HAi is an application provided by Hornbill and uses third-party AI Providers, including OpenAI and Azure OpenAI, for certain AI functionality. 

Certifications applicable to the underlying AI service apply to the relevant AI Provider and service rather than representing certification of the individual AI model or HAi itself.

OpenAI publishes information regarding its security and compliance certifications and controls, including SOC 2 Type 2 and ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, ISO/IEC 27701 and ISO/IEC 42001, as applicable to its services. For information, see OpenAI Security & Privacy.

HAi is governed by Hornbill's Subscription Agreement, applicable Data Processing terms and [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf), which incorporates the GDPR, UK GDPR and Data Protection Act 2018 into the applicable Data Protection Legislation governing HAi.

### How does HAi support data privacy and data-protection requirements?

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) defines applicable Data Protection Legislation as including the GDPR, UK GDPR and Data Protection Act 2018.

Where Customer Data contains Protected Data, the Customer instructs Hornbill to process that data for the additional purpose of providing HAI functionality and HAI Output. 

Hornbill uses AI Providers, including OpenAI and Azure OpenAI, to provide certain HAI functionality.

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) also places restrictions on the types of data that may be submitted to HAI unless the relevant HAI capability expressly supports its processing, and sets out requirements governing the use of Customer Data for improving HAI and AI model training.

### How is information about the use of personal data provided?

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) provides contractual information about the processing of Customer Data in connection with HAI, including the use of Customer Data as Input to HAI and the use of AI Providers to provide certain HAI functionality.

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) also states that the Customer is responsible for providing transparency and explainability notices required by applicable law.

### How can incorrect personal data be updated?

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) does not specify a separate HAI process for correcting personal data or handling data-subject rectification requests. 

As personal data resides in areas of Hornbill, outside of HAi, it is the responsibility of the customer to maintain their data across Hornbill.

### How can personal data be erased?

HAi does not retain a separate memory of personal data from previous interactions, and Customer Data is not used to train the underlying AI models. HAi processes each request using the relevant data available within Hornbill at the time the request is made.

As a result, there is no separate HAi data store from which personal data needs to be erased. Personal data is managed and retained within Hornbill in accordance with the Customer's established data-management and retention processes.

### How can the processing of personal data be stopped or restricted?

HAi provides customer-level controls that allow administrators to enable or disable HAi features and control which users are permitted to use HAi. Where supported, customers can also restrict the information made available to HAi to defined subsets of data.

These controls allow the Customer to restrict use of HAi and the data made available to it at an organizational or user-access level. However, HAi does not provide a mechanism to restrict the processing of an individual data subject's data independently of the applicable user or data-access controls.

### How can individuals object to the processing of their personal data?

Customers remain responsible for assessing and responding to objections to processing in accordance with applicable data-protection legislation and their established data-protection processes.

### How does HAi address automated decision-making?

HAi is designed to provide human oversight rather than make consequential decisions about individuals without human involvement.

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) expressly prohibits HAi being used as the sole basis for decisions that may materially affect an individual's legal rights, employment, financial position, health, safety or access to essential services without appropriate human review and oversight.

### How does HAi address profiling?

HAi generates responses and recommendations based on the Input and contextual information provided to the relevant HAi capability.

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) places responsibility on the Customer for establishing appropriate internal policies for the use of AI, ensuring that its use of HAI complies with applicable law, and providing required transparency notices and obtaining necessary consents.

### How does Hornbill maintain compliance as regulations and requirements evolve?

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) provides for updates to the HAI Terms where required, including updates required by law. 

Where a modification materially affects the Customer's rights or obligations, Hornbill will provide at least 30 days' prior written notice before the modification takes effect, subject to the exceptions set out in the [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf).

The [Hornbill Artificial Intelligence Agreement](https://www.hornbill.com/hubfs/Website/PDF/HAI%20Agreement.pdf) also permits Hornbill to modify, replace or discontinue third-party AI models, providers, services or technology where reasonably necessary for legal or regulatory reasons.