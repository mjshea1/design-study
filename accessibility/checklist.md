# Checklist

This checklist is from [Shift Nudge](https://shiftnudge.com), series of online learning courses. The workshop this came from was Designing Beautiful Interfaces.

## Accessibility Checklist

### Layout

* Have you used standardized controls and components in a very intentional way?
* If you haven't used standardized controls, do you have a very good reason? And have you talked to your developer about implementing it in an accessible way? _\(Example, auto-suggest lists have a specific way of being implemented to be screen-reader friendly\)_
* Can a user visually navigate a page in a logical way?
* Is there a clear page title that states the purpose of the page?
* Do the headers accurately convey the structure of information?
* Does the visual order match the reading order? \(Left to right, top to bottom\)
* Do the interface elements have appropriate labels? _\(Inputs, checkboxes, radio buttons, etc.\)_
* Do the clickable actions have clear action-oriented labels? _\(Download, Sign Up, Log Out, etc._
* `Developer` - Don't put status text or other non-interactive elements into the tab order
* `Developer` - Are you using the &lt;a&gt; and &lt;button&gt; tags appropriately? _\(They can both be triggered by Enter, whereas the &lt;button&gt; element can additionally be triggered with the Spacebar\)_
* `Developer` - Can a screen reader scan your project's interface? _\(A screen reader will announce headers, specific areas, links, buttons, and controls along the way\)_
* `Developer` - Do keyboard controls provide a logical and predictable order for navigation
* `Developer` - Have you defined [Roles](https://www.w3.org/TR/wai-aria/#document_structure_roles), [States, and Properties](https://www.w3.org/TR/wai-aria/#global_states)?

### Typography

* Is the text at a readable size? _\(Primary body copy no smaller than 16px\)_
* Do the titles and body copy have optimal line height?
* Do the paragraphs fall within the optimal character width of 45 – 75 characters? [https://readable.now.sh](https://readable.now.sh/)
* Have you considered how your design will _read_ if you closed your eyes and had someone describe what they see in a logical order?
* Have you considered the responsive nature of text-based content and created rules around truncation and or change of layout based on viewport?
* `Developer` - Are you using `<strong>` and `<emphasis>` appropriately with semantic markup?
* `Developer` - Have you considered creating a "large font size mode"? _Sometimes this can be done with creative develpment by using the mobile styles on larger viewports._

