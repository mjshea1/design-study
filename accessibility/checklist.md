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

### Color and Contrast

* Is information conveyed by means other than color alone? \(_Underlined links, status indicators, etc.\)_
* Does text meet the minimum contrast ratio requirements? \(3.0 for large text and informational graphics, 4.5 or higher for all other text\) [https://usecontrast.com/guide](https://usecontrast.com/guide) 
* `Developer` Have you considered creating alternate color themes or a high-contrast version? \(AAA–7.0 or higher for all text\) [https://whitehouse.gov/accessibility](https://whitehouse.gov/accessibility)

### Media

* Have you avoided text inside of bitmap graphics whenever possible?
* Have you made transcripts available for any audio files? _\(Helpful for the deaf and for people who aren't in a suitable environment to listen\)_
* Have you provided closed-captions _\(and transcriptions\)_ for any video content? _\(_[_Rev_](https://rev.com/)_,_ [_Descript_](https://descript.com/)_, etc.\)_
* `Developer` Have you checked your icons for a minimum AA Large \(3.0\) contrast? Have they been properly labeled via the interface design or within the code?
*  `Developer` Does all of your image-based content have alt \(alternate text\)?  _\(Also helpful if internet connection is slow\)_

### Functionality

* Have you provided feedback for user specific user interactions? _Clearly communicate what's happened, what can be done next, etc. Validation and error messages?_
* Have you made sure that no part of your interface flashes more than three times per second? _\(This can cause seizures\)_
* Make sure your site or app doesn't change context or activate functionality automatically. _\(Newsletter popups anyone?\)_
* `Developer` Have you provided identification for languages `<html lang="en">`?
* `Developer` Don’t automatically refresh an entire app canvas unless it is really necessary for app functionality. \(_Assitive technologies generally must assume that a page refresh is a totally new structure.\)_
*  `Developer` Have you used Accessibility tools to verify screen reading experience? \([Accessibility Insights](https://chrome.google.com/webstore/detail/accessibility-insights-fo/pbjjkligggfmakdaogkfomddhfmpjeni/related), [Axe](https://www.deque.com/axe/), etc.\)
*  `Developer` If you haven't used only native HTML, have you implemented the correct ARIA \(Accessible Rich Internet Applications\) roles to bridge the gap? \(_Note some HTML5 elements don't have accessibility support, so using both HTML5 elemtns and ARIA roles can be used to cover those gaps.\)_



