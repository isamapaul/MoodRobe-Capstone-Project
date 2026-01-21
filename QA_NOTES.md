## QA Build & Backend Validation Notes

### Backend Build Attempt
- Ran `npm run build`
- TypeScript compilation failed due to strict typing of Express route parameters
- Errors observed across Admin, Cart, Order, and Payment controllers

### Observation
- req.params values typed as `string | string[]`
- Use cases expect `string`
- Identified as integration-level type-safety issue

### Action Taken
- Documented findings
- Proceeded with static analysis of backend architecture and business logic
