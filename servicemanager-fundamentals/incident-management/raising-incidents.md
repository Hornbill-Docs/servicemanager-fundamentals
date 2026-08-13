# Raising Incidents

## Multiple ways to log an incident

Your team and your users shouldn't be limited to a single way of reporting an issue. With Hornbill, incidents can be logged manually by an agent, created automatically from an email arriving in a monitored mailbox, submitted by a user through a guided set of questions on the self-service portal, started from a chat conversation, or raised automatically from a monitoring or alerting tool. Incidents can also be raised directly from an existing service request or change record, so nothing gets lost as work moves between teams.

**Learn more:** [Intelligent Capture Designer](/servicemanager-config/customize/intelligent-capture-designer/) | [Email Routing Rules](/esp-config/email/using-email-routing-rules) | [Link Request Action](/servicemanager-user-guide/service-portfolio/requests/link-action)

## Incident templates for common issue types

Not every incident needs to start from a blank page. Administrators can define request catalog items that act as templates, pre-filling the category, priority, form fields, and questions for a particular type of incident — whether that's a routine password reset, a complex technical fault, a security incident, or an issue specific to a particular department or service. Different teams can each have templates tailored to how they work.

**Learn more:** [Using Workflows with Service Manager](/servicemanager-config/customize/workflows/using-workflows-with-service-manager)

## Incident models: templates plus workflow

A template tells the system what information to capture; an incident model goes a step further by pairing that template with its own dedicated workflow. This means a security incident, for example, can automatically follow a different journey — with its own approvals, tasks, and notifications — to a routine incident, without your service desk needing to remember which process applies.

**Learn more:** [Using Workflows with Service Manager](/servicemanager-config/customize/workflows/using-workflows-with-service-manager)

## Creating incidents from chat and virtual agents

Incidents can be created and updated directly from a live chat conversation, with the conversation captured in the incident record automatically rather than being retyped by an agent afterwards. Where a virtual agent (chatbot) is used — including through channels such as Microsoft Teams — incidents can be logged completely automatically, with the correct service, category, and details already applied, freeing your service desk from repetitive data entry.

**Learn more:** [Hornbill Virtual Agent](/hornbill-utilities/teams-power-virtual-agent) | [chatbotLogRequest (API reference)](/servicemanager-api-api/flowcodes/espflowcodeoperation/content/chatbotlogrequest)

## Spotting duplicate incidents

Before logging a new record, agents can use Hornbill's global search or the request list to quickly check whether a similar incident already exists, then link the new report to it rather than creating a duplicate. Where an issue is already known, agents can flag and link it in seconds, keeping reporting clean and avoiding wasted effort on the same problem.

**Learn more:** [Global Search for Requests](/servicemanager-user-guide/request-list/global-search-for-requests) | [Link Request Action](/servicemanager-user-guide/service-portfolio/requests/link-action)
