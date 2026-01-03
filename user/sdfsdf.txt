#include "kernel/types.h"
#include "user/user.h"

int
main(int argc, char *argv[])
{
  printf("ugetpid returned: %d\n", ugetpid());
  printf("uuptime returned: %d\n", uuptime());
  sleep(10);
  printf("uuptime returned: %d\n", uuptime());
  printf("getmem returned: %d\n", getmem());
  exit(0);
}