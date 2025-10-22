The assignment started with me cloning a prototype reddit repo.

Then I set up a GitHub App by following the instruction in the brief and also watching the provided video for more and concise understanding of the process.

And while doing this I was able to get my Auth GitHub ID and secret key for my .env file. 

While also trying to get my database url and password I was concerned about how to carry out this task without breaking my previous tables in my supabase. The current task required that i create tables with names that I already had in my previous tables. I checked with a senior developer who told me of 2 options to solve the problem.

1. To edit names of tables so it can work correctly (He however stated that this may cause some errors going forward if this was not correctly)
2. Signup on supabase with a new email. So I can start afresh without any conflicts with already existing tables.

He recommended option 2.

I therefore did as recommended by my senior developer.

While setting up the new account on supabase I faced an unfamiliar UI. Aparently supabase had changed their UI and I wasnt sure what to do as I did not know where to see the transaction pooler and I was starting to think that I may have done something wrong while setting up the new account. 

I sort the help of a senior developer who had a look at it with me. He also was seeing it for the first time, however, they say, knowledge shows the way but experience walks the path. We found the transaction pooler with his help and the database url was gotten and put correctly in the .env file as it should. 

I met another stumbling block when I tried to run my app. My terminal kept telling me that {session.user.name} was not defined. It also complained of missing secret key. This became a border as I was sure that I had put the keys from my github APP. The solution to this was to delete the suffix .example in the naming of the .env file.

What I learned from this particular experience is that even though the environment variables can be properly put in the .env file, if the file is not properly name then it will not work. What that showed was that there was NO ENVIRONMENT VARIABLE . 

Another reflection I have on this project is that after it was working properly in my localhost:3000, I deployed on vercel and when I tried to sign into the app it didnt go through. This was because the Homepage URL and the Callback URL in my GitHub App were carrying http://localhost3000 hence why I couldnt log in. 

A senior developer watched and directed me while I found out these bug and I fixed it by changing these URLs and putting the vercel domain url into the APP. This made login possible on the deployed APP.



🎯 Please mention the requirements you met and which goals you achieved for this assignment.
Apart from getting the APP deployed on vercel which was the basic task/requirement on this assignment, I was also able to Fix page titles on post pages to match the post title.

Again while doing this and having finished with my code for metadata needed for this task I thought I would be seeing the result immediately in my deployed version. I checked the metadata and could not see the result of the code. I was so certain it would work until a senior developer asked me if I had pushed my code to gitHub then I realised I was looking at the wrong place. He told me to make sure that in my code everything that needs to be awaited should be awaited. When I had a relaxed look at the code again I realised that I hadnt awaited one of my lines.

I corrected myself and tested locally and everthing worked perfectly as desired.


What I have learned from this exercise is that constant practice makes perfect coding. The other stretch goals not done by me could have been attempted better if I have practiced more. This is the penultimate week and I feel I am more knowledgeable. All I need is more practice to be able to attack assignments with more confidence. I am however proud of the journey so far. 