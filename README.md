
Marstek Venus E v3 Home Assistant Integration (Discontinued)

Project Status: Development Stopped

This repository is no longer being developed.  
After extensive testing, I found that the Marstek Venus E v3 Open not is currently not returning valid responses for certain requests — most notably:

```json
{
  "id": 1,
  "method": "Es.GetStatus",
  "params": {
    "id": 0
  }
}
````

Both firmware versions v137 and v139 fail to provide any response to this method, even though all other API calls work correctly.
This appears to be a firmware-level issue, not a problem with the integration code itself.

I have already performed multiple resets and factory restores without success, and v139 seems to be the latest firmware currently available from Marstek.

---

Recommended Alternative

Development has been discontinued here because https://github.com/jaapp/ha-marstek provides a much more advanced and actively maintained integration for the Marstek Venus E v3.

Jaap has done excellent work on improving communication with the API, and I fully trust his approach and future updates.
For the latest and most reliable integration, please visit and support his project instead.

---

Final NNote
Thanks to everyone who followed or tested this integration during development.
I truly appreciate the interest and feedback from the community.
From this point on, all future users are kindly referred tto Jaap’s rrepositor for continued updates and support.

— Christiaan2003


