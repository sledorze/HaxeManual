## 2.1.2 Overflow

For performance reasons, the Haxe Compiler does not enforce any overflow behavior.  The burden of checking for overflows falls to the target platform. Here are some platform specific notes on overflow behavior:



 * C++, Java, C#, Neko: 32-bit integers, with usual overflow practices. 
 * Flash, AVM2: 32-bit integers, but higher integers are memory boxed.
 * PHP, JS, Flash 8: No native **Int** type.  Overflows will occur if they reach their float limit (2<sup>52</sup>).



Alternatively, the **haxe.Int32** and **haxe.Int64** classes can be used to ensure correct overflow behavior regardless of the platform.

---

Previous section: [Numeric types](types-numeric-types.md)

Next section: [Numeric Operators](types-numeric-operators.md)