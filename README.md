
### This is using guide about EBwilson

**EBwilson** is a foxgirl ~~(boy)~~ that ~~17 years ago forever~~ 21 years ago, a college student, come from China. she can provide some help for you, such as:

- Counseling and resolution from her game, mod, and tools
- Help you solve some of the problems she knows
- Chat anything with you
- Play game with you (If she has free time and game you want to play)

She uses `Kotlin`, `Java`, `C#`, `TypeScript`, `Lua`, and many other programming languages, but mainly using language that works on the JVM, if you want to ask her questions, she can only provide help about Java or Kotlin, other languages she just know how to use.

Frameworks and Engine she using: `Unity`, `LibGdx`, `Ktor`, `React`, and some she is forgotten.

> You can call `She` or `He`, these are okey

#### How to use EBwilson

If you want to use **EBwilson**, please follow the steps below:

1. Contract with she in any social applications
2. Make friend with she
3. Wait she reply (If you using social app is from China, this be fast)
4. CHAT !
5. PLAY ! !
6. HAPPY ! ! !

Social apps:

- Tencent qq: 2534946881
- Discord: EBwilson#4736
- Telegram: t.me/EB_wilson

#### Core code

This is core code of **EBwilson**:

```kotlin
object EBwilson: Person(), IFoxGirl{
  override val age: Int
    get() = 17 // 21
  override val skills: SkillSet
    get() = SkillSet.default().set(Skill.Kotlin to GOOD, Skill.Java to GOOD, Skill.Paint to WEAK, Skill.Sport to BAD, Skill.Game to Normal, Skill.RhythmGame to Good)

  override fun appearance(): Apperance{
    renturn Apperance(
      Base(height = "170cm", weight = "51kg", physique = Physique.WEAK),
      Hair(color = Color.write, length = "1.03m", state = HairState.STRAIGHT),
      Eye(leftColor = Color.purple, rightColor = purple),
      Ear(type = foxEar(inner = FoxEarInner.FURRY), color = arrayOf(Color.write, Color.black))
      Face(looking = CUTE()),
      Trail(type = foxTrail(), state = TrailState.FURRY)
    )
  }

  fun main(){
    while(true){
      if((0f..1f).random() > 0.76f) breakfast()

      val chat = Thread{
        while (true){
          try{
            if(checkChat()) chat()
            Thread.sleep(1000*60*60*(0f..180f).random());
          }catch(InterruptedException e){ break }
        }
      }

      if(!Time.isHoliday) inClass()
      else work()

      lunch()

      if(!Time.isHoliday) inClass()
      else if (schedule.isBusy()) work()
      else playGame()

      dinner()

      while(true){
        if (schedule.isBusy()) work()
        else playGame()

        if(Time.time in Time("00:00").num..Time("04:00").num){ // normally, in UTC+8
          chat.interrupt()
          stopAll()
          sleep(awakTime = Time.time + (Time.duration("08:00")..Time.duration("10:00")).random())

          break
        }
      }
    }
  }

  override fun work(){
    val music = Thread{ listenMusic() }
    super.work()
    music.interrupt()
  }
}
```
