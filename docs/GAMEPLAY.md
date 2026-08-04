# TalkQuest Skill Tree

## Purpose

Skill Tree là hệ thống kỹ năng giao tiếp dùng chung cho toàn bộ TalkQuest.

Người học không chỉ hoàn thành từng bài riêng lẻ. Họ học một kỹ năng rồi tái sử dụng kỹ năng đó trong nhiều tình huống khác nhau.

Ví dụ:

Greeting
→ dùng trong School
→ dùng trong Coffee Shop
→ dùng trong Restaurant
→ dùng trong Airport
→ dùng trong Hotel

## Starter Skill Tree

### Level 1: Basic Communication

1. Greeting
2. Saying Goodbye
3. Introducing Yourself
4. Asking Someone's Name
5. Saying Thank You
6. Saying Sorry
7. Saying Yes and No
8. Asking for Help

### Level 2: Basic Information

9. Numbers
10. Age
11. Time
12. Days
13. Dates
14. Colors
15. Places
16. People

### Level 3: Daily Life

17. Family
18. School
19. Food
20. Drinks
21. Hobbies
22. Weather
23. Feelings
24. Daily Activities

### Level 4: Practical Communication

25. Ordering Food
26. Ordering Drinks
27. Shopping
28. Asking Prices
29. Asking Directions
30. Taking Transportation
31. Making Requests
32. Asking Permission

### Level 5: Real-Life Scenarios

33. Coffee Shop
34. Restaurant
35. Supermarket
36. Train Station
37. Airport
38. Hotel
39. Hospital
40. School Conversation

## Skill Structure

Mỗi skill phải có:

- Skill ID
- Name
- Description
- Level
- Vocabulary IDs
- Sentence Pattern IDs
- Example Dialogue IDs
- Required Skill IDs
- Scenario IDs
- Mission IDs
- Unlock Requirements

## Example Skill

Skill:

Greeting

Vocabulary:

- hello
- hi
- good morning
- good afternoon
- good evening

Useful Expressions:

- Hello!
- Hi!
- Good morning!
- How are you?
- Nice to meet you.

Used In:

- School
- Coffee Shop
- Restaurant
- Hotel
- Airport
- Meeting Friends

## Unlock Rule

Một skill có thể yêu cầu skill khác hoàn thành trước.

Ví dụ:

Greeting
→ Introducing Yourself
→ Asking Questions
→ School Conversation

## Important Rule

Không được sao chép cùng một skill vào nhiều bài học.

Mỗi skill chỉ có một nguồn dữ liệu chính.

Scenario và Mission chỉ tham chiếu đến Skill ID.
