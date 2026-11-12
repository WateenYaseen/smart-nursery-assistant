# T09 — AI Assistant Chat Interface

**Priority:** Medium  
**Estimate:** 1 working day  
**Status:** Planned

## Why

The owner needs a conversational interface to ask plant-care questions and receive guidance using relevant plant information when available.

## Done When

- The AI Assistant Chat screen follows the approved UI design.
- The screen displays a conversation area.
- The owner can enter and send a text message.
- User messages and assistant responses are displayed separately.
- A loading indicator appears while waiting for a response.
- A clear error message is displayed if sending or receiving a response fails.
- The interface supports Arabic RTL text.
- The assistant can receive the selected plant context when available.
- The conversation structure supports storing messages under a conversation identifier.
- An empty state displays a welcome message and example questions.

## Touches

- AI Assistant Chat screen.
- Message input component.
- Conversation interface.
- Assistant response component.
- Conversation and message data models.
- Selected plant context.
- Loading and error states.

## Notes

This ticket focuses on the chat interface and its basic conversation flow.

The final conversational AI provider and integration approach have not yet been selected. If the assistant service is not available, use a clearly identified placeholder response for interface testing.

Do not present placeholder responses as real AI-generated guidance.