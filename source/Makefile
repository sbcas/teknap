# Generated automatically from Makefile.in by configure.
# source/Makefile.in
#
# TekNap/source/Makefile
# Copyright Colten Edwards 1999

.SUFFIXES: .c .o .in .so

prefix = /usr/local
exec_prefix = ${prefix}
srcdir = .
#topdir = .
#incdir = ./include
#objdir = .
#bindir = ${exec_prefix}/bin
#datadir = ${prefix}/share
#libdir = ${exec_prefix}/lib
#libexecdir = ${exec_prefix}/libexec
#mandir = ${prefix}/man
#local_dir = $(HOME)


TARGET = TekNap

OBJECTS = alias.o alist.o array.o browse.o cdns.o commands.o compat.o debug.o \
	exec.o faccess.o files.o flood.o functions.o glob.o help.o history.o \
	hook.o if.o input.o ircaux.o ircsig.o keys.o lastlog.o list.o log.o \
	main.o md5.o mp3print.o mp3db.o napster.o network.o newio.o \
	output.o ptest.o reg.o screen.o scott.o scott2.o send.o server.o \
	setup.o share.o status.o term.o timer.o tgtk.o vars.o whois.o window.o \
	words.o xmms.o irchandler.o  $(CD_OBJS) $(MP3_OBJS)

#SOURCES = `echo $(OBJECTS) | sed -e 's/\.o/\.c/g'`
SOURCES = $(OBJECTS:%.o=%.c)

default:
	@echo ........... Making TekNap-$(_VERSION_) by panasync
	(cd ..;gmake)
	@echo ........... Done making TekNap-$(_VERSION_)

all: $(_VERSION_)

.c.o:
	$(CC) $(CFLAGS) $(DEFS) $(INCLUDES) -c $<

$(_VERSION_): $(OBJECTS) $(TCL_OBJS)
	$(CC) $(LDFLAGS) -o $@ $(OBJECTS) $(TCL_OBJS) $(LIBS)
clean::
	$(RM) $(_VERSION_) $(OBJECTS) sterm.* wterm.* $(TARGET)

clean::
	$(RM) *~ ../*~ ../include/*~ core a.out debug.out gmon.out $(TARGET)

# .o files needing special compilation flags

main.o: Makefile ../Makefile
	$(CC) $(CFLAGS) $(DEFS) $(INCLUDES) \
	-DNAPLIB=\"$(NAPLIB)\" -c $(srcdir)/main.c

screen.o: Makefile ../Makefile
	$(CC) $(CFLAGS) $(DEFS) $(INCLUDES) -c $(srcdir)/screen.c

mp3control.o: Makefile ../Makefile
	$(CC) $(CFLAGS) $(DEFS) $(INCLUDES) \
	-DMP3_PLAYER=\"$(MP3_PLAYER)\" -c $(srcdir)/mp3control.c

#
# dependencies
#

depend:
	@echo 'Making dependencies.  This takes a while'
	@sed -n '1,/^# Dont even THINK of deleting this line$$/p' < Makefile.in > tmp
	@mv -f tmp Makefile.in
	@gcc $(DEFS) $(CFLAGS) -E -MM $(SOURCES) >> Makefile.in
	@(cd ..;./config.status)

# Dont even THINK of deleting this line
alias.o: alias.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/alias.h \
 ../include/array.h ../include/commands.h ../include/history.h \
 ../include/hook.h ../include/input.h ../include/output.h \
 ../include/screen.h ../include/window.h ../include/lastlog.h \
 ../include/server.h ../include/status.h ../include/vars.h \
 ../include/ircterm.h ../include/scott.h ../include/stack.h \
 ../include/list.h ../include/keys.h ../include/newio.h \
 ../include/timer.h expr2.c expr.c
alist.o: alist.c ../include/alist.h ../include/teknap.h \
 ../include/defs.h ../include/config.h ../include/color.h \
 ../include/bsdglob.h ../include/irc_std.h ../include/ircaux.h \
 ../include/debug.h ../include/output.h
array.o: array.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/array.h ../include/ircaux.h \
 ../include/debug.h ../include/output.h
browse.o: browse.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/hook.h \
 ../include/list.h ../include/output.h ../include/newio.h \
 ../include/server.h ../include/timer.h ../include/napster.h \
 ../include/vars.h
cdns.o: cdns.c ../include/cdns.h ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/newio.h \
 ../include/commands.h ../include/output.h
commands.o: commands.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/alias.h \
 ../include/exec.h ../include/if.h ../include/history.h \
 ../include/hook.h ../include/keys.h ../include/list.h \
 ../include/input.h ../include/output.h ../include/ircterm.h \
 ../include/screen.h ../include/window.h ../include/lastlog.h \
 ../include/scott.h ../include/server.h ../include/vars.h \
 ../include/status.h ../include/stack.h ../include/napster.h \
 ../include/commands.h ../include/timer.h ../include/help.h \
 ../include/scott2.h ../include/tgtk.h ../include/whois.h \
 ../include/ptest.h ../include/newio.h ../include/irchandler.h \
 ../include/cdrom.h ../include/mp3control.h
compat.o: compat.c ../include/defs.h ../include/ircaux.h \
 ../include/teknap.h ../include/config.h ../include/color.h \
 ../include/bsdglob.h ../include/irc_std.h ../include/debug.h
debug.o: debug.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/hook.h \
 ../include/input.h ../include/output.h ../include/lastlog.h \
 ../include/screen.h ../include/window.h ../include/status.h \
 ../include/vars.h
exec.o: exec.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/exec.h \
 ../include/hook.h ../include/vars.h ../include/commands.h \
 ../include/window.h ../include/lastlog.h ../include/screen.h \
 ../include/input.h ../include/list.h ../include/server.h \
 ../include/output.h ../include/newio.h
faccess.o: faccess.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/ircaux.h ../include/debug.h
files.o: files.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/list.h \
 ../include/hook.h ../include/server.h ../include/commands.h \
 ../include/output.h ../include/vars.h ../include/scott.h \
 ../include/status.h ../include/window.h ../include/lastlog.h \
 ../include/newio.h ../include/napster.h
flood.o: flood.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/flood.h \
 ../include/hook.h ../include/output.h ../include/server.h \
 ../include/vars.h
functions.o: functions.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/alias.h \
 ../include/array.h ../include/files.h ../include/list.h \
 ../include/input.h ../include/napster.h ../include/newio.h \
 ../include/output.h ../include/ircterm.h ../include/screen.h \
 ../include/window.h ../include/lastlog.h ../include/scott.h \
 ../include/server.h
glob.o: glob.c ../include/config.h ../include/color.h \
 ../include/bsdglob.h ../include/defs.h ../include/ircaux.h \
 ../include/teknap.h ../include/irc_std.h ../include/debug.h
help.o: help.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/help.h \
 ../include/input.h ../include/hook.h ../include/output.h \
 ../include/screen.h ../include/window.h ../include/lastlog.h \
 ../include/server.h ../include/ircterm.h ../include/scott.h \
 ../include/vars.h
history.o: history.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/vars.h \
 ../include/history.h ../include/output.h ../include/input.h
hook.o: hook.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/alias.h \
 ../include/hook.h ../include/window.h ../include/lastlog.h \
 ../include/output.h ../include/stack.h
if.o: if.c ../include/teknap.h ../include/defs.h ../include/config.h \
 ../include/color.h ../include/bsdglob.h ../include/irc_std.h \
 ../include/struct.h ../include/alist.h ../include/ircaux.h \
 ../include/debug.h ../include/alias.h ../include/window.h \
 ../include/lastlog.h ../include/vars.h ../include/output.h \
 ../include/if.h ../include/commands.h
input.o: input.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/commands.h \
 ../include/exec.h ../include/history.h ../include/hook.h \
 ../include/input.h ../include/keys.h ../include/screen.h \
 ../include/window.h ../include/lastlog.h ../include/server.h \
 ../include/ircterm.h ../include/scott.h ../include/list.h \
 ../include/vars.h ../include/output.h ../include/status.h \
 ../include/napster.h
ircaux.o: ircaux.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/vars.h \
 ../include/screen.h ../include/window.h ../include/lastlog.h \
 ../include/output.h ../include/ircterm.h ../include/scott.h
ircsig.o: ircsig.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h
keys.o: keys.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/history.h \
 ../include/input.h ../include/keys.h ../include/output.h \
 ../include/screen.h ../include/window.h ../include/lastlog.h \
 ../include/ircterm.h ../include/scott.h ../include/vars.h
lastlog.o: lastlog.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/lastlog.h \
 ../include/window.h ../include/screen.h ../include/vars.h \
 ../include/output.h ../include/status.h
list.o: list.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/list.h
log.o: log.c ../include/teknap.h ../include/defs.h ../include/config.h \
 ../include/color.h ../include/bsdglob.h ../include/irc_std.h \
 ../include/struct.h ../include/alist.h ../include/ircaux.h \
 ../include/debug.h ../include/log.h ../include/vars.h \
 ../include/screen.h ../include/window.h ../include/lastlog.h \
 ../include/output.h
main.o: main.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/alias.h \
 ../include/commands.h ../include/exec.h ../include/hook.h \
 ../include/server.h ../include/status.h ../include/vars.h \
 ../include/input.h ../include/output.h ../include/ircterm.h \
 ../include/screen.h ../include/window.h ../include/lastlog.h \
 ../include/scott.h ../include/keys.h ../include/history.h \
 ../include/newio.h ../include/timer.h ../include/napster.h \
 ../include/cdns.h ../include/ptest.h ../include/tgtk.h \
 ../include/mp3control.h
md5.o: md5.c ../include/md5.h
mp3print.o: mp3print.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/napster.h
mp3db.o: mp3db.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/output.h \
 ../include/mp3db.h
napster.o: napster.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/keys.h ../include/struct.h \
 ../include/alist.h ../include/ircaux.h ../include/debug.h \
 ../include/commands.h ../include/flood.h ../include/hook.h \
 ../include/input.h ../include/list.h ../include/output.h \
 ../include/napster.h ../include/server.h ../include/status.h \
 ../include/window.h ../include/lastlog.h ../include/whois.h \
 ../include/vars.h ../include/ptest.h ../include/newio.h \
 ../include/scott2.h ../include/tgtk.h
network.o: network.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/cdns.h \
 ../include/newio.h ../include/ircterm.h ../include/screen.h \
 ../include/window.h ../include/lastlog.h ../include/scott.h \
 ../include/output.h ../include/vars.h
newio.o: newio.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/newio.h \
 ../include/output.h ../include/napster.h
output.o: output.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/log.h \
 ../include/output.h ../include/vars.h ../include/input.h \
 ../include/ircterm.h ../include/screen.h ../include/window.h \
 ../include/lastlog.h ../include/scott.h ../include/napster.h
ptest.o: ptest.c ../include/ptest.h ../include/teknap.h \
 ../include/defs.h ../include/config.h ../include/color.h \
 ../include/bsdglob.h ../include/irc_std.h ../include/struct.h \
 ../include/alist.h ../include/ircaux.h ../include/debug.h \
 ../include/newio.h ../include/output.h ../include/vars.h \
 ../include/if.h ../include/commands.h
reg.o: reg.c ../include/teknap.h ../include/defs.h ../include/config.h \
 ../include/color.h ../include/bsdglob.h ../include/irc_std.h \
 ../include/ircaux.h ../include/debug.h ../include/output.h
screen.o: screen.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/log.h \
 ../include/hook.h ../include/screen.h ../include/window.h \
 ../include/lastlog.h ../include/server.h ../include/status.h \
 ../include/output.h ../include/vars.h ../include/list.h \
 ../include/ircterm.h ../include/scott.h ../include/input.h \
 ../include/newio.h
scott.o: scott.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/commands.h \
 ../include/input.h ../include/list.h ../include/output.h \
 ../include/napster.h ../include/server.h ../include/status.h \
 ../include/window.h ../include/lastlog.h ../include/vars.h \
 ../include/scott.h ../include/scott2.h ../include/tgtk.h
scott2.o: scott2.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/scott2.h ../include/struct.h \
 ../include/alist.h ../include/ircaux.h ../include/debug.h \
 ../include/tgtk.h ../include/napster.h ../include/output.h \
 ../include/server.h
send.o: send.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/commands.h \
 ../include/hook.h ../include/list.h ../include/output.h \
 ../include/server.h ../include/vars.h ../include/status.h \
 ../include/window.h ../include/lastlog.h ../include/newio.h \
 ../include/napster.h
server.o: server.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/hook.h \
 ../include/list.h ../include/newio.h ../include/output.h \
 ../include/server.h ../include/status.h ../include/timer.h \
 ../include/vars.h ../include/window.h ../include/lastlog.h \
 ../include/napster.h ../include/scott2.h ../include/tgtk.h \
 ../include/irchandler.h
setup.o: setup.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/ircaux.h ../include/debug.h
share.o: share.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/input.h \
 ../include/list.h ../include/output.h ../include/md5.h \
 ../include/server.h ../include/status.h ../include/vars.h \
 ../include/window.h ../include/lastlog.h ../include/napster.h
status.o: status.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/ircterm.h \
 ../include/screen.h ../include/window.h ../include/lastlog.h \
 ../include/scott.h ../include/list.h ../include/server.h \
 ../include/status.h ../include/vars.h ../include/input.h \
 ../include/output.h ../include/napster.h
term.o: term.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/screen.h \
 ../include/window.h ../include/lastlog.h ../include/vars.h \
 ../include/ircterm.h ../include/scott.h ../include/output.h
timer.o: timer.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/lastlog.h \
 ../include/window.h ../include/timer.h ../include/output.h \
 ../include/commands.h ../include/vars.h ../include/server.h \
 ../include/screen.h
tgtk.o: tgtk.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/tgtk.h ../include/struct.h \
 ../include/alist.h ../include/ircaux.h ../include/debug.h \
 ../include/scott2.h ../include/newio.h
vars.o: vars.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/status.h \
 ../include/window.h ../include/lastlog.h ../include/history.h \
 ../include/napster.h ../include/log.h ../include/vars.h \
 ../include/input.h ../include/ircterm.h ../include/screen.h \
 ../include/scott.h ../include/output.h ../include/server.h \
 ../include/stack.h ../include/list.h ../include/ptest.h \
 ../include/newio.h ../include/cdrom.h
whois.o: whois.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/commands.h \
 ../include/hook.h ../include/if.h ../include/list.h \
 ../include/napster.h ../include/output.h ../include/server.h \
 ../include/cdns.h ../include/newio.h
window.o: window.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/exec.h \
 ../include/hook.h ../include/log.h ../include/screen.h \
 ../include/window.h ../include/lastlog.h ../include/server.h \
 ../include/vars.h ../include/list.h ../include/ircterm.h \
 ../include/scott.h ../include/input.h ../include/status.h \
 ../include/output.h ../include/napster.h
words.o: words.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/ircaux.h ../include/debug.h
xmms.o: xmms.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/alias.h
irchandler.o: irchandler.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/irchandler.h \
 ../include/list.h ../include/napster.h ../include/output.h \
 ../include/server.h ../include/window.h ../include/lastlog.h \
 ../include/vars.h
cdrom.o: cdrom.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/cdrom.h \
 ../include/output.h ../include/vars.h
mp3control.o: mp3control.c ../include/teknap.h ../include/defs.h \
 ../include/config.h ../include/color.h ../include/bsdglob.h \
 ../include/irc_std.h ../include/struct.h ../include/alist.h \
 ../include/ircaux.h ../include/debug.h ../include/exec.h \
 ../include/hook.h ../include/napster.h ../include/newio.h \
 ../include/output.h
