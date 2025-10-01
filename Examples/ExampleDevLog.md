# 🗓️ Developer Log – 2025-09-26 - 2025-09-28

## 🛠 What I Worked On

* Solved NeetCode’s **ThreeSum** (medium) and **Container With Most Water** (medium).

  * ThreeSum: initially summed indices instead of values — fixed by using `nums[i] + nums[j] + nums[k]`. Practiced pointer movement and duplicate skipping.
  * Container: focused on shrinking window approach, learned to move the shorter side to maximize area.
* Finished building the **student analytics page** off a coworker’s branch. Types between branches were inconsistent, so I modularized and cleaned them up for reusability.
* Met with **Frontend B team** → created a strategy for merging analytics page and dashboard with minimal conflicts.
* Cleaned up repository structure → consolidated source code into `src/` folder for clarity.
* Added **PRDs** to the project → documented tasks needed for analytics + dashboard so future devs have context.

## 📚 What I Learned

* **Next.js router basics**: navigating between pages with `useRouter()`.
* **Prefetching**: how to preload routes for faster transitions.
* **Dynamic routes in Next.js**: accessing params from the URL (`[id].tsx` pattern).
* Noticed **Cursor’s output patterns** → tends to create many inline functions. Planning to refactor these into shared utils for reuse.

## ✅ What Went Well

* Scheduled early-week strategy session with team → reduced merge conflicts and created a smoother release plan.
* **Pseudocoding NeetCode problems** in the morning made me more productive during commutes and breaks → solved 2 problems faster than last week.
* Dedicated one night purely to ticket work (no distractions) → deep work led to cleaner implementation of dashboard features.
* Improved **collaboration with Cursor** → instead of copy-pasting, I reviewed generated code and identified reusable patterns.

## 🚧 What Blocked Me

* Couldn’t check in with backend team → uncertain if the types I created match real data. Current `data.ts` file feels bloated due to assumptions made with Emily. Might require rework once actual API is finalized.

## 🔜 Next Steps

* Debug data visualization feature and request team feedback tomorrow morning.
* Reach out to backend team for type validation to reduce redundancy in `data.ts`.

## 📝 Notes / Reflections

* 🧠 **Workflow:** Want to optimize for deep work *daily*, not just weekends. I’ll try journaling coding sessions in a notebook to better capture micro-progress.
* 🤝 **Networking:** Realized I default to going home after work instead of attending events. Want to schedule at least one networking event per week (e.g., Code & Coffee follow-ups).
* 🛠 **Coworking:** Interested in organizing coworking with friends. Need to experiment with balancing focus time + collaborative learning.
* 🎯 **Metrics:** This week → 2 NeetCode mediums solved, 1 repo cleanup, 1 analytics feature completed. Next week, aim: +3 LeetCode problems and backend type sync.
