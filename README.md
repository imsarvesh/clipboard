# clipboard



import type { CodegenConfig } from '@graphql-codegen/cli';

const config: CodegenConfig = {
  overwrite: true,
  schema: "http://localhost:3000/api/graphql",
  documents: "Queries/**/*.ts",
  generates: {
    "types/typeDefs.d.ts": {
      plugins: ["typescript", "typescript-operations"],
    },
    "./graphql.schema.json": {
      plugins: ["introspection"],
    },
  },
};


//"codegen": "graphql-codegen --config codegen.ts"

export default config;


    "codegen": "graphql-codegen --config codegen.ts"
    
    "@graphql-codegen/cli": "4.0.0",
    "@graphql-codegen/introspection": "4.0.0",
    "@graphql-codegen/client-preset": "4.0.0"
    
    

Defination of ready
1. For Bug: Detail steps to reproduce (video or picture will be helpful too)
2. For Enhancement: Detail steps to verify the enhancement or change.  It will also be helpful to provide sample accounts. (But do not include password in radar, use attache)
3. For sub-task radars, please state “No QA required” and mention the parent radar instead.


Defination of Done
1. Requirement document attached?: <Yes/No> , Reviewed: <Yes/No> 
2. Test plan attached?: <Yes/No> , Reviewed: <Yes/No> 
3. Followed Simple coding guidelines? : <Yes/No>
4. SonarLint checked? : <Yes/No>
5. Dev testing done based on the test plan?: <Yes/No>
6. Screen recording or screenshot for the fix attached? : <Yes/No> , Reviewed: <Yes/No> 
7. Ticket Tracked in UAT, Prod : <Till where its tracked> or we can make Yes/No
