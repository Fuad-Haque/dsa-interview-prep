# DSA Interview Prep

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Sora&weight=700&size=22&duration=2800&pause=1000&color=6C63FF&center=true&vCenter=true&width=700&lines=140+Problems.+19+Concepts.+1+Ladder.;Arrays+%C2%B7+Graphs+%C2%B7+DP+%C2%B7+Caching+%C2%B7+Rate+Limiting;Ordered+DSA+prep+for+Production+LLM+Engineering+loops;Built+for+climbing+the+ladder%2C+not+skipping+around.)](https://git.io/typing-svg)

</div>

<div align="center">

![Scope](https://img.shields.io/badge/Scope-Production_LLM_Engineering-6C63FF?style=for-the-badge)
![Concepts](https://img.shields.io/badge/Concepts-19-6C63FF?style=for-the-badge)
![Problems](https://img.shields.io/badge/Problems-140-DC244C?style=for-the-badge)
![Remote](https://img.shields.io/badge/Remote-US%2FEU-007ACC?style=for-the-badge)

</div>

---

## Overview

**DSA Interview Prep** is a personal interview-preparation checklist for Production LLM Engineering loops (remote, US/EU), organized by *concept* and ordered easiest → hardest rather than grouped by source or shuffled randomly. Each of the 19 sections represents one recurring interview concept (arrays & hashing, sliding window, graphs, dynamic programming, caching, rate limiting, and so on), and every item inside is a single interview question phrased exactly as it would be asked live, with no hints, no solutions, and no pattern notes attached.

The goal isn't to jump to the hardest-sounding question first — it's to climb the ladder concept by concept, confirming the fundamentals before layering on the LLM/backend-infra concepts (15–19) that show up specifically in AI-infrastructure loops.

**Repository** → [github.com/your-username/dsa-interview-prep](https://github.com/your-username/dsa-interview-prep)

---

## Table of Contents

- [Features](#features)
- [Structure](#structure)
- [Concepts](#concepts)
- [Item Naming Convention](#item-naming-convention)
- [Quick Start](#quick-start)
- [Project Structure](#project-structure)
- [Progress Tracker](#progress-tracker)
- [Notes on Repeated Problems](#notes-on-repeated-problems)
- [Author](#author)

---

## Features

| Feature | Detail |
|---|---|
| Concept-First Ordering | 19 numbered sections, ordered easiest → hardest, isolating one core concept instead of mixing concepts by source |
| Core + Infra Split | Concepts 1–14 are the classic SWE-loop core; concepts 15–19 are the LLM/backend-infra layer specific to AI-infra loops |
| Live-Phrased Questions | Every item is phrased exactly as it would be asked live — no hints, no solutions, no pattern notes |
| Ordered Within Section | Each concept's problems are also ordered easiest → hardest, so a section is itself a mini-ladder |
| Follow-Up Chains | A handful of sections (e.g. Rate Limiting, Caching) are explicitly designed as one live follow-up chain rather than independent problems — see [Notes on Repeated Problems](#notes-on-repeated-problems) |
| Self-Contained Checklist | Each item is a standalone checkbox — track progress inline, no external tracker needed |

---

## Structure

```
Concept Section (e.g. 01_Arrays_And_Hashing)
│
├── Problem 1  → two_sum.py
├── Problem 2  → valid_anagram.py
├── Problem 3  → contains_duplicate.py
├── Problem 4  → group_anagrams.py
├── Problem 5  → maximum_subarray.py
├── Problem 6  → product_of_array_except_self.py
├── Problem 7  → top_k_frequent_elements.py
├── Problem 8  → longest_consecutive_sequence.py
├── Problem 9  → single_number.py
└── Problem 10 → intersection_of_two_arrays_ii.py
```

Every one of the 19 sections follows this same shape: a batch of items, one concept, increasing difficulty within the section (basic warm-up vs. rotated/streamed/bounded-memory variant, multiple valid approaches, follow-up escalation, etc.) so the concept gets tested from a few different angles rather than just once.

---

## Concepts

| # | Folder | Concept | Core Idea |
|---|---|---|---|
| 01 | `01_Arrays_And_Hashing` | Arrays & Hashing | Trade space for O(1) lookups to find pairs, duplicates, and groupings in a single pass |
| 02 | `02_Two_Pointers` | Two Pointers | Converge two pointers from opposite ends to prune the search space on sorted or symmetric input |
| 03 | `03_Sliding_Window` | Sliding Window | Expand/contract a window over a sequence to satisfy a length, count, or distinctness constraint |
| 04 | `04_Stack` | Stack | Match, validate, or evaluate nested/sequential structures using a LIFO stack |
| 05 | `05_Binary_Search` | Binary Search | Reason about invariants over a sorted or monotonic search space in O(log n) |
| 06 | `06_Linked_List` | Linked List | Reverse, merge, or restructure pointers iteratively, recursively, or in place |
| 07 | `07_Recursion_And_Backtracking` | Recursion & Backtracking | Explore/prune a decision tree to enumerate subsets, permutations, or combinations |
| 08 | `08_Trees_Binary_Tree_BST` | Trees (Binary Tree / BST) | Recursive traversal, path-sum, LCA, and serialization over binary trees and BSTs |
| 09 | `09_Heap_Priority_Queue` | Heap / Priority Queue | Maintain a min/max-heap to solve top-k, k-way merge, and running-median problems |
| 10 | `10_Tries` | Tries | Prefix-based tree structure for word storage, wildcard search, and board-based word lookup |
| 11 | `11_Graphs` | Graphs | BFS/DFS, topological sort, and union-find over grids and general graphs |
| 12 | `12_Intervals_And_Greedy` | Intervals & Greedy | Sort by start/end and sweep to merge, insert, or greedily resolve overlapping intervals |
| 13 | `13_1D_Dynamic_Programming` | 1-D Dynamic Programming | Bottom-up DP with O(1) or O(n) state, building on prior subproblems along a single axis |
| 14 | `14_2D_Dynamic_Programming` | 2-D Dynamic Programming | Grid or two-string DP tracking state across two dimensions simultaneously |
| 15 | `15_Design_Data_Structures` | Design / Data Structure Implementation | Compose multiple data structures correctly under constant-time and capacity constraints |
| 16 | `16_Caching_LRU_LFU` | Caching (LRU / LFU) | Hash map + doubly linked list (or frequency buckets) to implement O(1) eviction policies |
| 17 | `17_Rate_Limiting_Token_Bucket` | Rate Limiting & Token Bucket | Fixed window, sliding log/counter, and token bucket algorithms for per-user request throttling |
| 18 | `18_Streaming_Parsing_Buffers` | Streaming, Parsing & Buffers | Buffer, chunk, and reconstruct partial reads, ring buffers, and length-prefixed byte streams |
| 19 | `19_Concurrency_Bounded_Queues` | Concurrency & Bounded Queues | Blocking bounded queues, producer-consumer systems, and semaphore-based concurrency limiters |

---

## Item Naming Convention

Every checklist item maps to a `snake_case` identifier, derived directly from the question's subject:

```
Given an array of integers, return indices of two that sum to target   → two_sum.py
Design a Least Recently Used (LRU) cache with O(1) get/put             → lru_cache.py
Find the kth largest element in an unsorted array                      → kth_largest_element_in_an_array.py
```

Where an item is explicitly a follow-up or harder variant of an earlier one (e.g. sliding-window log vs. fixed-window counter rate limiting), the variant suffix is kept as-is rather than collapsed into the base name, so `token_bucket_rate_limiter.py` stays distinct from `sliding_window_rate_limiter.py`.

---

## Quick Start

Clone the repository:

```bash
git clone https://github.com/your-username/dsa-interview-prep
cd dsa-interview-prep
```

Work through any individual section directly:

```bash
open 01_Arrays_And_Hashing/README.md
```

No dependencies, environment, or solutions included — this is a question ladder, not a solved-problem archive. Solve top to bottom, concept by concept, and don't skip around.

---

## Project Structure

```
dsa-interview-prep/
├── 01_Arrays_And_Hashing/
│   ├── two_sum.py
│   ├── valid_anagram.py
│   ├── contains_duplicate.py
│   ├── group_anagrams.py
│   ├── maximum_subarray.py
│   ├── product_of_array_except_self.py
│   ├── top_k_frequent_elements.py
│   ├── longest_consecutive_sequence.py
│   ├── single_number.py
│   └── intersection_of_two_arrays_ii.py
├── 02_Two_Pointers/
│   ├── valid_palindrome.py
│   ├── two_sum_ii.py
│   ├── three_sum.py
│   ├── trapping_rain_water.py
│   ├── container_with_most_water.py
│   └── is_subsequence.py
├── 03_Sliding_Window/
│   ├── best_time_to_buy_and_sell_stock.py
│   ├── longest_substring_without_repeating_characters.py
│   ├── longest_repeating_character_replacement.py
│   ├── permutation_in_string.py
│   ├── minimum_window_substring.py
│   └── sliding_window_maximum.py
├── 04_Stack/
│   ├── valid_parentheses.py
│   ├── min_stack.py
│   ├── evaluate_reverse_polish_notation.py
│   ├── largest_rectangle_in_histogram.py
│   ├── decode_string.py
│   └── generate_parentheses.py
├── 05_Binary_Search/
│   ├── binary_search.py
│   ├── search_a_2d_matrix.py
│   ├── search_in_rotated_sorted_array.py
│   ├── find_minimum_in_rotated_sorted_array.py
│   ├── first_bad_version.py
│   └── median_of_two_sorted_arrays.py
├── 06_Linked_List/
│   ├── reverse_linked_list.py
│   ├── linked_list_cycle.py
│   ├── merge_two_sorted_lists.py
│   ├── add_two_numbers.py
│   ├── remove_nth_node_from_end_of_list.py
│   ├── reorder_list.py
│   ├── copy_list_with_random_pointer.py
│   ├── reverse_nodes_in_k_group.py
│   └── merge_k_sorted_lists.py
├── 07_Recursion_And_Backtracking/
│   ├── fibonacci_number.py
│   ├── subsets.py
│   ├── permutations.py
│   ├── combination_sum.py
│   ├── word_search.py
│   ├── palindrome_partitioning.py
│   └── n_queens.py
├── 08_Trees_Binary_Tree_BST/
│   ├── invert_binary_tree.py
│   ├── maximum_depth_of_binary_tree.py
│   ├── same_tree.py
│   ├── balanced_binary_tree.py
│   ├── subtree_of_another_tree.py
│   ├── lowest_common_ancestor.py
│   ├── binary_tree_level_order_traversal.py
│   ├── binary_tree_right_side_view.py
│   ├── validate_binary_search_tree.py
│   ├── kth_smallest_element_in_a_bst.py
│   ├── construct_binary_tree_from_preorder_and_inorder.py
│   ├── diameter_of_binary_tree.py
│   ├── serialize_and_deserialize_binary_tree.py
│   └── binary_tree_maximum_path_sum.py
├── 09_Heap_Priority_Queue/
│   ├── kth_largest_element_in_a_stream.py
│   ├── last_stone_weight.py
│   ├── k_closest_points_to_origin.py
│   ├── kth_largest_element_in_an_array.py
│   ├── merge_k_sorted_lists_heap.py
│   ├── task_scheduler.py
│   └── find_median_from_data_stream.py
├── 10_Tries/
│   ├── implement_trie.py
│   ├── add_and_search_word.py
│   └── word_search_ii.py
├── 11_Graphs/
│   ├── number_of_islands.py
│   ├── clone_graph.py
│   ├── rotting_oranges.py
│   ├── walls_and_gates.py
│   ├── course_schedule.py
│   ├── course_schedule_ii.py
│   ├── min_cost_to_connect_all_points.py
│   ├── cheapest_flights_within_k_stops.py
│   ├── number_of_operations_to_make_network_connected.py
│   └── accounts_merge.py
├── 12_Intervals_And_Greedy/
│   ├── merge_intervals.py
│   ├── insert_interval.py
│   ├── non_overlapping_intervals.py
│   ├── employee_free_time.py
│   ├── minimum_number_of_arrows_to_burst_balloons.py
│   ├── gas_station.py
│   └── jump_game.py
├── 13_1D_Dynamic_Programming/
│   ├── climbing_stairs.py
│   ├── house_robber.py
│   ├── house_robber_ii.py
│   ├── longest_palindromic_substring.py
│   ├── palindromic_substrings.py
│   ├── coin_change.py
│   ├── longest_increasing_subsequence.py
│   ├── maximum_product_subarray.py
│   ├── word_break.py
│   └── partition_equal_subset_sum.py
├── 14_2D_Dynamic_Programming/
│   ├── unique_paths.py
│   ├── longest_common_subsequence.py
│   ├── edit_distance.py
│   ├── triangle_minimum_path_sum.py
│   ├── maximum_length_of_repeated_subarray.py
│   ├── minimum_path_sum.py
│   └── wildcard_matching.py
├── 15_Design_Data_Structures/
│   ├── min_stack.py
│   ├── lru_cache.py
│   ├── freq_stack.py
│   ├── design_twitter.py
│   ├── design_hashmap.py
│   ├── flatten_2d_vector.py
│   ├── insert_delete_getrandom_o1.py
│   └── basic_calculator.py
├── 16_Caching_LRU_LFU/
│   ├── lru_cache_from_scratch.py
│   ├── lfu_cache.py
│   ├── lru_cache_with_ttl.py
│   ├── thread_safe_lru_cache.py
│   └── memory_bounded_llm_response_cache.py
├── 17_Rate_Limiting_Token_Bucket/
│   ├── fixed_window_counter.py
│   ├── sliding_window_log.py
│   ├── token_bucket.py
│   ├── sliding_window_counter.py
│   ├── per_tier_rate_limiter.py
│   └── distributed_rate_limiter.py
├── 18_Streaming_Parsing_Buffers/
│   ├── read_n_characters_given_read4.py
│   ├── read_n_characters_given_read4_ii_call_multiple_times.py
│   ├── stream_token_word_buffering.py
│   ├── ring_buffer.py
│   ├── length_prefixed_message_parser.py
│   ├── sse_stream_parser.py
│   └── token_budget_truncation.py
└── 19_Concurrency_Bounded_Queues/
    ├── bounded_blocking_queue.py
    ├── producer_consumer_system.py
    ├── priority_bounded_queue.py
    ├── task_scheduler_worker_pool.py
    ├── llm_batching_queue.py
    └── semaphore_from_scratch.py
```

---

## Progress Tracker

| Range | Concepts | Focus Area |
|---|---|---|
| 01 – 07 | Arrays, Two Pointers, Windows, Stack, Search, Lists, Backtracking | Core single-structure patterns — hashing, pointers, windows, and recursive enumeration |
| 08 – 14 | Trees, Heaps, Tries, Graphs, Intervals, 1-D & 2-D DP | Recursive and multi-step structures — traversal, top-k selection, and dynamic programming |
| 15 – 19 | Design, Caching, Rate Limiting, Streaming, Concurrency | LLM/backend-infra layer — the Production LLM Engineering-specific loop concepts |

| Concept | Problems | Status |
|---|---|---|
| 1. Arrays & Hashing | 10 | ☐ |
| 2. Two Pointers | 6 | ☐ |
| 3. Sliding Window | 6 | ☐ |
| 4. Stack | 6 | ☐ |
| 5. Binary Search | 6 | ☐ |
| 6. Linked List | 9 | ☐ |
| 7. Recursion & Backtracking | 7 | ☐ |
| 8. Trees | 14 | ☐ |
| 9. Heap / Priority Queue | 7 | ☐ |
| 10. Tries | 3 | ☐ |
| 11. Graphs | 10 | ☐ |
| 12. Intervals & Greedy | 7 | ☐ |
| 13. 1-D DP | 10 | ☐ |
| 14. 2-D DP | 7 | ☐ |
| 15. Design | 8 | ☐ |
| 16. Caching (LRU/LFU) | 5 | ☐ |
| 17. Rate Limiting | 6 | ☐ |
| 18. Streaming & Parsing | 7 | ☐ |
| 19. Concurrency & Queues | 6 | ☐ |
| **Total** | **140** | |

---

## Notes on Repeated Problems

A few problems intentionally appear in more than one section, since they're valid entry points for more than one concept:

| Problem | Sections | Why |
|---|---|---|
| `merge_k_sorted_lists.py` / `merge_k_sorted_lists_heap.py` | `06_Linked_List`, `09_Heap_Priority_Queue` | Solvable with pairwise two-list merging or with a min-heap across all lists — the heap version is the explicit follow-up when asked to optimize past brute-force merging |
| `min_stack.py` | `04_Stack`, `15_Design_Data_Structures` | Same constant-time-getMin stack, cross-listed once as a stack warm-up and once under the explicit "design" framing companies use to introduce constrained-API problems |
| `lru_cache.py` / `lru_cache_from_scratch.py` | `15_Design_Data_Structures`, `16_Caching_LRU_LFU` | The design-round version accepts any O(1) approach; the caching-round version explicitly requires hand-building the hash map + doubly linked list rather than using built-in ordered-dict shortcuts |

Each appearance is a deliberate re-ask using that section's specific framing or constraint, not a duplicate item left in by accident. The Rate Limiting (17) and Streaming/Parsing (18) sections go a step further — within each of those sections, treat every item as one continuous live follow-up chain rather than independent problems, since that's how these are reported to actually run in the loop.

---

## Author

Built by [Fuad Haque](https://github.com/Fuad-Haque)

[GitHub](https://github.com/Fuad-Haque)
