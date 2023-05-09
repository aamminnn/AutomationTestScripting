# AutomationTestScripting
Experience in Automation Test Scripting on Television Software

Hi all!
As you can see I cannot include the code as it is confidential
but I can share the idea of my experience.

There are 2 flowcharts which is automation flowchart and judgement flowcharts. Imma break it down.

For Automation flowchart, it describe the general flow of test scripting.

[Read and understand test plan requirement] Firstly, I read and understand the requirement of the test plan. Mostly the testplan looks kinda the same pattern but as I handle for many regions, there is a lot difference to take note. On average each test plan has at least 20 test cases to be automated.

[Skimming] Due to time and energy constraint, I then skimmed the test plan to check wether the test case able to be automated or worth to be automated. In some condition where testcase cannot be automated is when additional hardware is needed, for example amplifier or smart card.

[Develop, shakedown, debug] After I filtered all the testcase to be automated, then I start to develop the test script. The idea of starting develop the test script is I write all the test script without testing the TV software just to check wether my code runable or not. If my script got issue, I debug and fix the issue first before I actually running on the software.

[Test validation] After script is completed, then I run a full test on the software. In some cases one testcase takes a very long time at least 3-4 hours to complete, in that case I run them one by one. The result depends on how many test case pass or fail. The way I analyse is to see the result pattern. If the fail is consistent, there might be software issue and need to be reported. If the fail scatters and happen at random, there might be intermitent error or script issue, then I go on debugging. Repeat the process until one test plan completed.


For Judgement Flowcharts, it describes how judgement and results is produced.
The way the TV software is tested is basically using text and picture judgement. Mostly text judgement. The idea is when the test script run, until certain checkpoint, it will capture the TV screen, for example channel information. Channel information display various of information of the channel (Channel name, Channel number, Time, Channel description, Age rating etc). 

The screen captured is judged by some prebuilt function. 
Although I don't know the details of the function, but basically the idea is on the screen, the function will create some area to be detected(argument of the function), text in the area will be read, using neural network to compare the text either the text match or not with the expected text we put into argument of the function. If the text match, the result will pass, else it will fail.
