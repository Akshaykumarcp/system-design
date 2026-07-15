# system-design
System Design Resources

## Resources
- [hello interview](https://www.hellointerview.com/), [YT](https://www.youtube.com/@hello_interview)
    - [System Design]((https://www.hellointerview.com/learn/system-design/in-a-hurry/introduction))
        - [Delivery](https://www.hellointerview.com/learn/system-design/in-a-hurry/delivery)
        - [core cocepts](https://www.hellointerview.com/learn/system-design/in-a-hurry/core-concepts)
        - [community questions](https://www.hellointerview.com/community/questions?sort=recentAndPopular&page=1)
        - Problem breakdowns
            - [Uber](https://www.hellointerview.com/learn/system-design/problem-breakdowns/uber)
            - [Rate Limiter](https://www.hellointerview.com/learn/system-design/problem-breakdowns/distributed-rate-limiter)
        - Patterns
            - [Real-time Updates](https://www.hellointerview.com/learn/system-design/patterns/realtime-updates)
        - Blogs
            - [Mastering Estimation](https://www.hellointerview.com/blog/mastering-estimation)
        - Mock Interviews
            - [Design an e-commerce platform](https://youtu.be/RuGY_1pap74?si=I2l1_Yfs-0esLrFs)
                - feedback:
                    - articulate on why elastic search
                        - preindexed so faster
                        - built in search
                        - pressure on primary db is eased out
                        - sync with primary db is CDC
                    - cache regular queries
                    - talk about multiple options and trade off during design
                        - using domestic concurrency control vs redis cache during DB
                        - DCC needed for edge cases
                    - find an area of design where really talk about trade off description
                    - for price change:
                        - CDC into queue -> workers -> two choices -> 1. put into another queue for fanout on changes. sub for product change. 2. capture product. can leverage another queue for real time notification. use pub-sub. stopped. watch video
                    - scale services required
                    - do proper dive deep on scale and functional requirement
                    - failure scenarios, edge cases, observability and gaurantability  after functional and non-functional requirements
                        - redis may blow up
                            - relay on OCC
                        - pub-sub, have primary and seconday 
                        - come up with 2 or 3 and solve them
                    - capture sometime on non-functional req
                        - latency
                            - capture time ppl sub and time of prod has changed and time sent notification
                    - spend quality time on detail solution and close solution
                    - slow down the pace at high level and deep dive
                        - focus on providing quality content
                        - do not explain not required
                        - ex: here solution on concurrency should work for explaining more
    - [Low-Level Design](https://www.hellointerview.com/learn/low-level-design/in-a-hurry/introduction)
    - [ML System Design](https://www.hellointerview.com/learn/ml-system-design/in-a-hurry/introduction)
    - Blogs:
        - [Staff-Level System Design](https://www.hellointerview.com/blog/staff-level-system-design)
    - [Practice](https://www.hellointerview.com/practice/overview)


        


