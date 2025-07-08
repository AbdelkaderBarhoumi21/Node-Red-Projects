# Node-RED Demo Flows

This repository contains a comprehensive collection of Node-RED flows organized into multiple tabs, each illustrating key core and advanced features:

## Tabs / Topics

1. **Fundamentals**  
   - Basic use of `inject`, `debug`, `change`, `switch`, `join`, `split`, `range` nodes  
   - Demonstrates simple message transformations, conditional routing, array handling, and unit scaling

2. **Arranging Flow**  
   - Use of **Groups**, **Comments**, **Junction** and **Link** nodes  
   - Best practices for visually organizing and modularizing complex flows

3. **Link Call Flow**  
   - Example of inter-tab communication using **link in**, **link out**, and **link call** nodes  
   - Implements a “multiply by 2” subflow to show return-link patterns

4. **Building Complex Flow**  
   - Storing and retrieving values in **flow** and **global** context  
   - Capturing start/end timestamps and computing elapsed time

5. **Context Store**  
   - Managing a simple “family presence” registry in global context  
   - Link-in/out subflows to update/read shared data

6. **Environment Variables**  
   - Switching behavior between `production` and `development` modes via `env.get("MODE")`  
   - Example of hot-swappable environment-dependent routing

7. **Function Node**  
   - Advanced JavaScript examples: arithmetic, if/else, loops, status updates  
   - Splitting arrays into multiple messages, and custom node status indicators

8. **Complete Node & Error Handling**  
   - Using the **complete** node to detect when async functions finish  
   - Structured error handling with **catch** and per-type routing

9. **Websocket Server**  
   - Simple WebSocket input/output integration  
   - Debugging live message streams

10. **Subflows**  
    - A reusable “Supabase Query” subflow that:  
      - Connects to a Supabase database via `@supabase/supabase-js`  
      - Accepts `Table`, `Filter Property`, and `Filter Value` as environment parameters  
      - Emits loading, success, or error status messages

11. **UI Dashboard**  
    - **ui_form**, **ui_dropdown**, **ui-table**, **ui-chart**, **ui-slider** examples  
    - Dynamically querying Supabase and rendering results in tables and charts  
    - Demonstrates two tabs: default and “Supabase dashboard”

12. **Securing Node-RED**  
    - Using **ui-control** to monitor user events (e.g. login/logout)  
    - A baseline for adding route protection, authentication, or audit logging

---

## How to Use

1. **Import** the JSON into your Node-RED editor.  
2. Install required npm packages for function nodes:  
   ```bash
   npm install @supabase/supabase-js weather-js
