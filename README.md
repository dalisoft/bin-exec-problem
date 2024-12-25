# Binary execution speed improvement

## Motivation

I am driven to enhance the performance and reduce the startup execution times of development tools such as `pre-commit`, `pre-push`, and similar processes. These optimizations are not limited to local environments but also extend to Continuous Integration and Continuous Deployment (CI/CD) pipelines. Here's why this is important:

1. **Faster Development Workflow:**

    - **Local Efficiency:** By speeding up tools like `pre-commit` and `pre-push`, developers can experience quicker feedback loops. This means less waiting time when committing or pushing code, leading to a more seamless and productive workflow.
    - **CI/CD Performance:** Optimizing these processes in CI/CD pipelines ensures that automated tests and deployments run faster, accelerating the overall development cycle.

2. **Cost Reduction:**

    - **CI/CD Costs:** Faster execution times in CI/CD pipelines can lead to reduced usage of computational resources. This efficiency can translate to lower costs, especially when using cloud-based CI/CD services that charge based on resource consumption.
    - **Local Resource Savings:** Improving execution times on local machines means that less computational power is required, which can decrease electricity usage and prolong hardware lifespan.

3. **Energy Conservation and Environmental Impact:**

    - **Battery Life:** For developers working on laptops or portable devices, optimized processes consume less power, thereby extending battery life and enhancing mobility.
    - **Carbon Footprint:** Reduced energy consumption not only benefits individual users but also contributes to lowering the overall carbon footprint. Efficient CPU usage means less electricity is needed, which is beneficial for both the environment and energy conservation efforts.

4. **Performance and Resource Optimization:**

    - **CPU Efficiency:** By making these tools run more efficiently, we can ensure that the CPU is utilized optimally without unnecessary strain. This leads to smoother performance of other applications running concurrently.
    - **Sustainability:** Efficient software practices align with broader sustainability goals, supporting initiatives to reduce energy consumption and promote environmentally friendly computing.

In summary, my motivation is rooted in creating a more efficient, cost-effective, and environmentally responsible development ecosystem. By improving the performance of essential development tools and processes, I aim to benefit both individual developers and the larger community, while also contributing positively to environmental sustainability.

## Attempt 1

> [!CAUTION]
> Status: Failed or Rejected

Date: April 07 - April 09 at 2024

### Title: Find `platform` `bin` and replace link to that `bin`

### Alt title: Direct bin call

### Issues or Discussions

| Project  | Issue or Discussion                                    |
| -------- | ------------------------------------------------------ |
| dprint   | https://github.com/dprint/dprint-plugin-json/issues/35 |
| biomejs  | https://github.com/biomejs/biome/discussions/2315      |
| jsona    | https://github.com/jsona/jsona/issues/52               |
| lefthook | https://github.com/jsona/jsona/issues/52               |

### Solutions provided

| Project | PR                                           |
| ------- | -------------------------------------------- |
| dprint  | https://github.com/dprint/dprint/pull/839    |
| dprint  | https://github.com/dprint/dprint/pull/840    |
| biomejs | https://github.com/biomejs/biome/pull/2359   |
| oxc     | https://github.com/oxc-project/oxc/pull/2920 |

### Excepted

Like this solution: https://github.com/evanw/esbuild/blob/main/lib/npm/node-install.ts

## Attempt 2

> [!CAUTION]
> Status: Failed or Rejected

Date: April 12 - April 15 at 2024

### Title: Using `platform` packages `bin` and require by `engines`

### Alt title: Link `platform` `bin` to project main `package`

### Issues or Discussions

| Project  | Issue or Discussion                                 |
| -------- | --------------------------------------------------- |
| lefthook | https://github.com/evilmartians/lefthook/issues/703 |

### Solutions provided

| Project  | PR                                                |
| -------- | ------------------------------------------------- |
| lefthook | https://github.com/evilmartians/lefthook/pull/705 |

## Attempt 3

> [!CAUTION]
> Status: Failed or Rejected

Date: July 30 - August 01 at 2024

### Title: shell `bin.sh` solution to execute

### Issues or Discussions

| Project  | Issue or Discussion                               |
| -------- | ------------------------------------------------- |
| biomejs  | https://github.com/biomejs/biome/discussions/2315 |
| lefthook | https://github.com/jsona/jsona/issues/52          |

### Solutions provided

| Project  | PR                                                |
| -------- | ------------------------------------------------- |
| biomejs  | https://github.com/biomejs/biome/pull/3550        |
| lefthook | https://github.com/evilmartians/lefthook/pull/798 |
