# Motion for Svelte (motion-sv)

This skill provides expert knowledge for using `motion-sv`, a port of the Motion library (formerly Framer Motion) specifically designed for Svelte 5 using Runes.

**Crucial Difference:** This library aligns closely with the **motion-vue** API (e.g., using `inViewOptions` instead of `viewport`, and `whilePress` instead of `whileTap`), ensuring better compatibility with Svelte's reactivity system.

## Usage

This skill is automatically discovered by Claude when you request animations, transitions, or gestures within a Svelte 5 project, or when you explicitly mention `motion-sv`.

## Key Capabilities

-   **Core Components**: `<motion.div>`, `<AnimatePresence>` (with modes: sync, wait, popLayout).
-   **Layout Animations**: Handles the specific `createLayoutMotion` pattern required for Svelte (replaces React's snapshot system).
-   **Styling**: Enforces object syntax `style={{ ... }}` for correct MotionValue binding.
-   **Reorder**: Drag-and-drop list functionality (`ReorderGroup`, `ReorderItem`).
-   **Performance**: `LazyMotion` for code-splitting.
-   **Hooks**: `useSpring`, `useMotionValue`, `useTransform`, `useAnimate`.

## Critical Patterns

-   **Layout**: Use `createLayoutMotion(motion)` proxy for layout animations.
-   **Runes**: Built for Svelte 5 `$state` and `$effect`.
-   **API Naming**: `inViewOptions`, `whilePress`, etc.

## Sources & Credits

Based on the work of Haniel Ubogu.

-   **Repository:** [github.com/HanielU/motion-sv](https://github.com/HanielU/motion-sv)
-   **Based on:** [Motion (Framer Motion)](https://motion.dev/)
