# Project01
리파지토리 연습 &amp; git hub 작동 방식 테스트

```mermaid
flowchart TB
    A[지윤성]
    B("나야~")
    A ---> B
    B --test--> A
    A --> C{hello}
    B ---> C
```

```mermaid
flowchart LR
    calc([calc])
    calc --> inp[/입력/]
    inp --> out[/출력/]
    out --> rt([rt])

    start([start]) --> inp1[/입력/]
    inp1 --> fun1[[calc]] 
    %% 네모 겹친 것은 함수 호출 %%
    fun1 --> end1([end])

    start1([start]) --> blank((" "))
    blank --> cond{i < 4}
    cond -->|no| blank
    cond -->|yes| end2([end])
    one -->|재귀|one
    subgraph one["for i = 1; i < 30; i++"]
        direction TB
        subgraph two
            direction RL
            h1 --> h2
        end
        a1-->a2
    end
```