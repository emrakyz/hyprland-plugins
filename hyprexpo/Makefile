CXX = clang++

all:
	$(CXX) -shared -fPIC main.cpp overview.cpp OverviewPassElement.cpp -o hyprexpo.so -g \
	`pkg-config --cflags pixman-1 libdrm hyprland pangocairo libinput libudev wayland-server xkbcommon` \
	-std=c++2b -Wno-narrowing -stdlib=libc++ -lc++abi
clean:
	rm ./hyprexpo.so
