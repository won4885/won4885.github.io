---
layout: post
title: "[Java] Programmers 행렬의 덧셈"
tags: [algorithms, java, programmers]
gh-repo: daattali/beautiful-jekyll
comments: true
---

<https://programmers.co.kr/learn/courses/30/lessons/12950>

<br>

## Solution

```java
import java.util.Arrays;

class Solution {
    public static int[][] solution(int[][] arr1, int[][] arr2) {
        int[][] answer = new int[arr1.length][arr1[0].length];
        // int[][] answer = {};
        // answer = arr1;

        for (int i = 0; i < arr1.length; i++) {
            for (int j = 0; j < arr1[0].length; j++) {
                answer[i][j] = arr1[i][j] + arr2[i][j];
            }
        }

        return answer;
    }
}
```