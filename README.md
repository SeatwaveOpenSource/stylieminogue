<html>
  <head></head>
  <body>
    <img width="400px" src="https://github.com/SeatwaveOpenSource/stylieminogue/blob/master/logo.png" />
    <p>These guidelines are currently at their very early stages but should be followed for all new projects and existing projects should be changed where possible.</p>
    <p>If you want to make a change to these guidelines pull request it up!</p>
    <h2>Code Style</h2>
    <h3>C#</h3>
    <ul>
      <li>Spaces over Tabs
        <ul>
          <li>4 Spaces</li>
          <li>1 tab should insert 4 spaces</li>
        </ul>
      </li>
      <li>Always include access modifiers</li>
      <li>Underscores '<span style="color: rgb(0,0,255);">_</span>' should be used for private fields</li>
      <li>Regions should not be used</li>
      <li>Pascal case for public methods e.g.
          <pre>
public bool Store(string words)
{
    //code here
}</pre>
      </li>
      <li>Camel case for private methods e.g.
          <pre>
private bool store(string secrets)
{
    //code here
}</pre>
      </li>
      <li>No braces for single line conditionals
      <pre>
if (true)
    return false;</pre>
      </li>
      <li>Shorthand conditionals should ideally be one line
      <pre>
var friesWithThat = hungry ? "yes" : "no";</pre>
      </li>
      <li>Shorthand conditionals that are more than one line
      <pre>
var friesWithThat = hungryAPI.GetCurrentStomachStatus() == "Starving"
    ? foodAPI.EatJunkFood()
    : foodAPI.EatASalad();</pre>
      </li>
      <li>Summary XML should only be used for libraries
      <pre>
/// &ltsummary&gt
/// Class level summary documentation goes here.&lt/summary&gt
/// &ltremarks&gt
/// Longer comments can be associated with a type or member 
/// through the remarks tag&lt/remarks&gt
public class Burger
{
    /// &ltsummary&gt
    /// Description for GetBurgerName.
    /// &lt/summary&gt
    /// &ltparam name="order"&gt Parameter description for order goes here&lt/param&gt
    /// &ltseealso cref="Order"&gt
    /// You can use the cref attribute on any tag to reference a type or member 
    /// and the compiler will check that the reference exists. &lt/seealso&gt
    public string GetBurgerName(Order order)
    {
        return burgerAPI.GetBunType(order);
    }</pre>
    </li>
    </ul>
    <h3>JSON</h3>
    <ul>
      <li>Spaces over Tabs
        <ul>
          <li>2 Spaces</li>
          <li>1 tab should insert 2 spaces</li>
        </ul>
      </li>
    </ul>
    <h3>XML</h3>
    <ul>
      <li>Spaces over Tabs
        <ul>
          <li>4 Spaces</li>
          <li>1 tab should insert 4 spaces</li>
        </ul>
      </li>
    </ul>
  </body>
</html>