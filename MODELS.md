# Models

## QuestionPool

`[]Question`

The primary question pool has N=32. Presented QuestionPool will be randomly shuffled, and its order reconstructed at the
end of the questionnaire when the user reviews their answers.

For an "active" questionnaire, three pools will be maintained:
1. Unpresented Questions: These are the questions the user has not yet seen, and represents the initial QuestionPoo.
2. Answered Questions: These are the questions the user has seen and answered satisfactorily. They should be in the same
   order as the Unpresented Questions.
3. Presented Questions: These are the questions that have been presented to the user, and that the user has opted to
   return to later, or have seen at least once, but answered with a "question mark." These questions will be presented
   to the user in a random order. They must be presented at least once to the user before `?` becomes a valid option.


## Question

```json
{
  "id": 1,
  "presentedOrder": 5,
  "text": "I am a sample question. Am I a sample question?",
  "answer": null
}
```
