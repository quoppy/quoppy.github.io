layout: true
class: center, middle, black
---
background-image: url(images/title.jpg)

# Bits and Bugs
## or: How I Became a Software Engineer

???

Hello everyone. My name is Jay, and I am a software engineer at Lucasfilm.

I am here today to share a little of what I do, and how I got in to, what I
think, is one of the coolest companies around.

For those of you who are not familiar with Lucasfilm, what we mainly do in
Singapore is create...

---
background-image: url(images/lockdown.jpg)

???

giant robots...

---
background-image: url(images/whisperer.jpg)

???

dinosaurs...

---
background-image: url(images/hulkbuster.jpg)

???

and superheroes.

---
background-image: url(images/winter-before.jpg)

???

We create visual effects for movies, which means turning this...

---
background-image: url(images/winter-after.jpg)

???

...into what you see in the cinema.

---
background-image: url(images/destroyer.jpg)

???

As a software engineer, I design and write tools for the company to create
these beautiful images.

These tools can vary from something as simple as a website that helps
departments exchange information, to a sort-of internal Youtube for artists to
find and view each other's work.

It depends entirely on what the company needs to deliver the highest quality it
can as efficiently as possible.

---
class: left

.left[
```python
from tornado.httpclient import ASyncHTTPClient
import tornado.gen, tornado.ioloop, tornado.web

class GoodDog(tornado.web.RequestHandler):
    """Fetches things for a living."""

    def __init__(self, name='Max'):
        self.name = name
        
    @tornado.gen.coroutine
    def get(self, url1, url2, url3):
        http_client = AsyncHTTPClient()
        response1, response2 = yield [http_client.fetch(url1),
                                      http_client.fetch(url2)]
        response_dict = yield dict(response3=http_client.fetch(url3),
                                   response4=http_client.fetch(url4))
        response3 = response_dict['response3']
        response4 = response_dict['response4']
        print "Woof, %s got %s responses!" % (self.name, len(response_dict))

if __name__ == "__main__":
    application = tornado.web.Application([(r"/", GoodDog)])
    application.listen(8888)
    tornado.ioloop.IOLoop.current().start()
```
]

???

I don't have a set work routine. Most of my time is spent looking at things like
this.

This is source code.

You can think of it as a set of instructions that the computer will follow.

With enough code, you can create an app, a game, or Facebook. You can control a
smartphone, or send a space ship billions of kilometers away to take photos of
another planet. Or allow us to share what used to be only in our imagination.

To me, the most amazing thing is that I can make the computer do what I want.

Big programs can consist of thousands of lines of code, with many people working
on different parts at the same time.

Companies like Google and Facebook have thousands of software engineers all
around the world.

We are slightly smaller, less than a hundred over 4 countries.

In general, software enginners need logical thinking and problem-solving skills.
An effective engineer can break a large problem down into smaller,
simpler-to-solve parts.

Everything you're learning now is important because it is the foundation. Maths
and science appear very often in computing problems. Humanities like history
and literature are needed in video games and movies.

You also need to be able to speak well. It is no use being brilliant if no one
can understand what you're saying.

Speaking well is not using cheem words or an ang moh accent. It means being able
to convey your thoughts simply and precisely.

---
background-image: url(images/direction.jpg)

???

Now, the story of how I got to where I am today is slightly unconventional.

Let's go back 15 years to the year 2000. I was where someone of you will be
soon: after my O-Levels.

Back then, many parents and families, mine included, held this view.

After O-Levels, you go to JC. After JC you go university to become a lawyer,
doctor, banker or engineer.

The civil service is good too, because it's an iron rice bowl. Most like you
would have a job for life if you stay out of trouble and don't mess up.

Some of you might still be hearing it today from your parents.

So naturally off I went to JC.

The thing is, I had an interest in computers since I was young.

I knew what I wanted to learn, and that a polytechnic would teach me more than a
JC ever could.

In those days, a polytechnic was where you went when you were not good enough
for JC. Nowadays, it's a legitimate choice.

Of course, I'm not saying everyone should go poly. It's great only if you know
exactly what you want.

When I went home one day and told my mom that I wanted to go to poly, she was...

---
background-image: url(images/vegetable.jpg)

???

stun like vegetable. My relatives and teachers were also quite surprised when
they found out. Most didn't understand why.

I managed to persuade my mom that it was for the best. I would still be able to
get a degree, and was not throwing away my future on a whim.

Eventually, my poly results were good enough that the government paid me to go
to Australia to study computer science after NS.

At the time, this was like huat ah. I get to go overseas and study what I've
always wanted for free!

---
background-image: url(images/attached.jpg)

???

I didn't think too much about it then, but when you take the government's money,
there are always strings attached.

I had to pay them back with 6 years of working in the civil service.

After coming back to Singapore, I  started off as a Prisons Officer.

A year later, I moved on to the Ministry of Home Affairs to work on public
policy.

---
background-image: url(images/fence.jpg)

???

While it was meaningful, well-paying work, I wasn't happy.

After 3 years, I couldn't see myself doing this for another 3 years, much less
the rest of my life.

Emails, organising meetings, researching policies. It just wasn't for me. I
wasn't using anything I'd studied.

I was faced with another choice. Do I stay where I am? Or do I give up a good
career path and pay, leave and do something that would make me happy?

Again, my family and relatives were concerned. First I went to poly, not enough.
Now I want to destroy my iron rice bowl. I was basically shattering every 
pre-conceived notion they held about a sensible career.

---
background-image: url(images/road.jpg)

???

Spoiler alert: I quit.

Unfortunately as it turns out, 3 years in the civil service doesn't give you
many transferable skills.

I didn't have much luck finding a job in a software company because I lacked
relevant professional experience.

A friend then suggested Lucasfilm, who had an entry-level position. It was meant
for fresh graduates, the pay wasn't great and the work slightly menial.

But that didn't matter to me. First, it would be a foot in the door and a 
stepping stone to better things. Second, it's Star Wars!

I worked my way up for 2 years. After a long journey, I'm finally doing what
I've always wanted.

---
background-image: url(images/clouds.jpg)

### passion

### curiosity

???

Let me leave you with 10 words that I feel have been a good guide for me:
passion and curiosity.

My passion for computers and technology is what pushed me, and still pushes me
to do what I do every day. I don't go to work on Monday wishing it's Friday.

Being curious leads you to improve your knowledge. The first thing you learn
when you start working is that you know nothing. The sooner you realise that,
the better. You'll be humble and always be willing to learn something new.

When I first started at Lucasfilm, I had to learn a whole new world of visual
effects. Asking questions, both to myself and to others, made me learn a lot
faster than just being spoon-fed information.

I hope I've given you something to think about today, whether it's your future,
your possible choices, or why I said 10 when there are only 2 words. If you're
curious, find out how computers count.

Thank you.
