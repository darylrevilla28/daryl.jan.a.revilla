Additional Questions:

1. You are given a requirement which states "The system should scale to 2000 users". What other questions would you need to ask in order to get enough information to create a workload model?

[ANSWER:]
Given that the system can scale up to 2000 users, the questions that needs to be asked are:
1.) How many steps are there in each business flow?
2.) What is the target transaction/volume (per hr/min/sec) that needs to be achieved?
3.) What is the ramp-up rate?
4.) How long should the test run? 

2. Please rewrite the requirement above so that it is more descriptive and testable?

[ANSWER:]
Requirements:

Using Apache JMeter with your choice of language and framework, write a performance test script to complete the following:
 1. Load DuckDuckGo Homepage (https://duckduckgo.com/)
 2. Type Suggested Search Term
 3. Select Search Term from the suggested Search Box

The script should iterate all 3 transactions and cycle through the search terms located in the file SearchTerms_DuckDuckGo.txt picking a different one on each iteration.

The test needs to run for 5 minutes of sustained period with a target transactions of 30 iterations per minute

Each user should be treated as a new user and caching should be handled appropriately.

Your scripts should be in a complete and runnable state. Prepare the script as if it was being delivered to a client. Feel free to add anything else that that you would.

Each transaction should be measured (homepage, suggested search, search)

It is important to type the search term while recording so that the suggested search populates, do not cut and paste.


3. As well as creating a script in a tool to do the performance testing, what other factors would need to be considered for a performance testing engagement?

[ANSWER:]
Planning and Analyze Phase
- Performance Test Environment is already built and in stable condiction once the team is engaged. 
- Test Environment should be exclusive for Performance Testing only, especially on the Scripting and Test Execution phase. Test scripts may be affected if the environment keeps on changing and having new code drops every now and then, thus it requires additional effort to re-create the scripts from scratch
- All identified test scenarios in scope for performance testing are fully functional and working, any major defects will affect the overall performance testing timeline. 
- Perf Test Environment is a production like copy, in terms of server specifications, configurations, and volume of data in the database. 
- Client team will provision a virtual machine/VMWare/CITRIX or the like to the performance testing team provided with admin rights to install the performance testing tool needed. 

Test Design and Preparation 
- Test IDs and other necessary test data will be created and provided by the development team or equivalent team to the performance testing team. 
- No functional blockers that impacts any of the business process in scope.
- Performance Testers may seek assistance to functional testing team to clarify some of the steps in the functional test script. 
- Performance Testers may seek assistance to dev team if any functional blockers occurs preventing the team from creating the performance testing scripts. 
- Type of Performance Testing to be conducted. 

Performance Test Execution 
- Server monitoring will be conducted by the performance testing team provided the team was access to their monitoring tools. 
- Test Results analysis will be provided after each test execution 
- Fix related to major performance issue that will affect the timeline and will lead to additional test conduct needs to be escalated promptly. 
- Project Development Team will be handling performance fine tuning and performance defect fixes.















