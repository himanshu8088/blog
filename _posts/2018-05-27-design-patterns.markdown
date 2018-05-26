---
layout: post
title:  "Design Patterns"
date:   2018-05-27 00:00:00 +0530
categories: design-patterns
---

Strategy Pattern:

{% highlight ruby %}
namespace DesignPatterns.SingletonDP
{
    public sealed class Singleton
    {
        private static readonly Singleton _instance = new Singleton();

        private Singleton()
        {
        }

        static Singleton()
        {
        }

        public static Singleton Instance
        {
            get
            {
                return _instance;
            }
        }
    }

     public class Console{

        public static void Main(string[] args){
            // You would get same instance when each time using:
            Singleton singleton = Singleton.Instance;
        }
    }
}
{% endhighlight %}

