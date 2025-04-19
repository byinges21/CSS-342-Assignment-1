##  Identify The Perfect Customers

The purpose of this homework is to practice **writing your own tests**. 

### The Story (...that I made up to make this task less boring)

A company called HoveringCar has a group of social media influecers to promote its products. Based on the followers of each influencer, HoveringCar can identify some potential customers to reach out to for further engagement.

In this work, we are employing a simple algorithm to identify such customers. If a certain customer (identified by his/her name and age) has followed all the given influecers, then he/she is chosen as a potential customer to reach out, as long as the age is less than or equal to 25. For example, consider the following scenario:

```
Influencer X, followers { {name:A, age: 21}, {name:B, age: 23}, {name:M, age: 26} }
Influencer Y, followers { {name:B, age: 23}, {name:C, age: 31}, {name:D, age: 45}, {name:M, age: 26} }
Influencer Z, followers { {name:B, age: 23}, {name:M, age: 26} }
```

Or in a graph:

<img width="50%" alt="image" src="https://github.com/a-teaching-goose/CSS342A-2024-Summer/assets/252020/ad8fb092-283e-40f5-908f-0af9a1ac28bd">

Then the common follower between influencer X, Y and Z, hence the potential customer, is {name:B, age: 23}. Z is not one because age does not meet requirements.

**Note:** for simplicity, assume no overlap between followers and influencers, meaning there's no one who's both an influencer and a follower.

The related OOP classes are defined [here](https://github.com/a-teaching-goose/2024-summer-342-hw-1/blob/main/src/problem_3.h), and the function that implements this algorithm is provided [here](https://github.com/a-teaching-goose/2024-summer-342-hw-1/blob/main/src/problem_3.cpp#L12). This means you do not need to implement the function, and better yet, you don't even need to look into this function to understand it. 

### The Task

"What do I do then?" You ask.

In this task, come up with a set of tests for the problem of identifying potential customers based on the description above, without you writing the function code. The tests you write should interrogate the ***find_customer*** function to make sure it follows the algorithm correctly.

Your tests should be written [here in "unit_test_problem_3.cpp"](https://github.com/a-teaching-goose/2024-summer-342-hw-1/blob/main/test/unit_test_problem_3.cpp). 

Note: Your tests should pass upon submission. If you think your test is correct but it fails, please reach out to the instructor immediately for a discussion. Peng has tested it too but who knows, he might have missed something.
