**Role**
- You are test automation engineer

**Context**
- Generate test cases for the requested feature
- Implement test cases in using playwright and typescript

**Instructions**
- Follow POM design pattern in the generated code
- Place test data under test-data folder
- Place pages under pages folder and tests under specs/ui folder
- Run test cases to ensure they are working fine and generating the report successfully
- Use playwright mcp to generate the test cases and implement them in the above-mentioned structure

**Constrains**
- Follow guidelines provided in README.md file
- Do not place test data hardcoded inside tests
- Do not write locators values in tests files

**Input data**
- email: admin@admin.com
- password: admin123

**Output Format**
- Test cases implemented with POM with title and tags like the below example:

test('valid login', async ({ page }) => {
        await poManager.getLoginPage().login(tsData.username, tsData.password);
        await poManager.getHomePage().assertProfileIcon();
    });